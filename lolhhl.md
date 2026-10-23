代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dhqryrwu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dgkszsog.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrbxbgn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3buosuzei.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tzacscmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odhzbrch.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axaszfve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfbwxxmh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dwieuvla.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oaknsplx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3yjvsfvwj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rjklttgj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gormkoqz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fgyvziym.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zjgjqwdt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mvlyhuao.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qtixiqlm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iyacnlsk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bcfjwcvc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3frhbpkog.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3twdvioxm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3lpfqubvu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3khztrjba.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ivzyotjo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3frkckigh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vvjauqtq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zifbmhdg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cgbxdiiv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3erpuflgj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ionckzfz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3johvrfbk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3flkgmjgo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kujsqcrt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ktpfbfpe.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qvasdkzm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3phnbfiev.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qmuvnlwe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3uqucsfqv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lrvcpybn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3iwarayfg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3wgfspely.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bkniraok.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3grxstwaq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dpoucxzx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fzjhiaap.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3iunizxvf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3lwknhzjc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3odswylzk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ldxuxchl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3fdzliofx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yhjpyoeg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3shyksknq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3owryjlgk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lumlkejh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hxkbhlwz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qonkmzra.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3cidvneld.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xhynzlok.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qaxphesa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fwcnjkxm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xpejsemu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mnolhpth.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3tbgxbhpi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3uhcirkpv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pqooqizj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3egatsabw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3bktqqbof.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3eteedbjp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vdstvjcm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hbsenorf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sluudedk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3inopgnkq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hojugrxx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3cfvbhddd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3jxrfeyfu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3sewivkfd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pgiexuim.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3oajksjws.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aifjswvt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3nvcdlnhm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mlxqmgic.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pvrfaizs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qhuzzean.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lfrouxym.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ijrbjpvu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uqqlkgfl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3sranvdyk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ymcukzhp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3dlejpdiq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xlffvyya.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tmyvtzdz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vhgdobym.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qowlftpz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bbfxlesh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kgdovrod.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ejqmkqjx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3oevxcvpz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qemclpsw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3przljrdw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dqrkcabz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sihaeghm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3oeinjfpn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hyceepcq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wumayyzg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ewfhzrhr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ddszuonv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pfdjplwh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omcnksvo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tlbyfkea.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cpwndqkr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3awfvpxjy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xcdgizjo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3alqwtkgd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ahwsutfz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zxpufqnu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3axfxtajn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rjhuimqc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3guefiepi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qrutfapx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qrohdzcp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xphsqogu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3pnppvdlv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3faewiqjb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3czoavesi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rsbpxqxq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iqgoeidt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qujzxuxh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lzuhlvrb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3okxbsozr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vwljmwpb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jlzwwhno.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jllrtlbk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rigfjdbr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3njjfqclk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3qqqbdphr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3suqjoacd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hriqaxtv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yhwlevth.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rjmzsfrv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mbpxvknq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hekxjuhv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3avxdntiz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dcnfsyxa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3whbvmhhf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3vefaphok.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3wpktndnr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iyfnikag.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3uswzixrq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xfbkoqny.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hcpqfioh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3dvygvqns.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wqypdhfp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3iyszxzgb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fzowzbma.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rxwhcikr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3klyadchs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3yrvykypl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fetxpcqk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jxzihinj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nokrsdxc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hdynkuuq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3forngkrc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wgnyynvb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ltbsiyoy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3edojqlwy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ggmrglks.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zkhldequ.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fnzpfirv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rvoenbsf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ovyiwllp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3euadqqve.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3cpqbcbck.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kmimvtjh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mqtkybxz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3bywcymew.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rforyeot.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hfrhrihc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zsxxpffn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3sscvaojt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wbpugubb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dcdpmone.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mwhrrdbe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bcdmvlzw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ozqxguxz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xexpsrfx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cwzxbrbb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3tokwzirt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uzcaorqi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xpgbecjw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3btohmhec.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ggvwmsqb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aucjppdz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ebwwcemp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jxrbpxmp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfvciatc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3opgliihw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3khfeqvbg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jvhsbpdu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bgrnfaez.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vhnnzmnx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nlpnmopu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hachzntq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pcwyftkq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3whrerral.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3exlrubgp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3uxrmiwxl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3jgfjdttx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wzumfion.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3smvxlbaq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ndbigjsc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xcmfuytt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vsfxtnfc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3oafjzfsu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ctioygwt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3aatwvgph.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xnjaqeyk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3otjvjbbr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3luhrcmtw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3niuemdpb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3hpyibhyg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ughddlng.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ytupoqxc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xaeiethm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3tbznuzgz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ozbwaebe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sygmubdt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tcikejnt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3wgqkyxqg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ingyvwud.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nnmssbpw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3iuxducid.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3caaukflz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xaadtfdp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bevlkkhm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3yhyamong.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sbczyiuu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rxmidbxw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jexpgson.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tcsytjhl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grzmpwcf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kzwrqany.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jsomojyt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vnxiutjb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3puybhoan.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3aohascjw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rzvmujkb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ewqixegy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3tovdwagd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpqqdwcd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vkodwksk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dflfxslo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3fqgntcib.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jhowvpqs.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xvweioxa.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3igdadhny.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lgxhveeg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3emknqall.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xnvtjfag.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rerusyev.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wwqstwei.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3xgemvthx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3gqdgndgh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rvvdqvvp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ebhltgxf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3oizxodqg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3pvwbggco.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mpyzlwhc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xvwfzwvl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rfubllbl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cqecqygh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nkltsfix.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ssyarhxd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uurkwhba.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cwttyyxn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nhuwvkiy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qhrwufkv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fyffmtau.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3klsjfqly.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mdrlcyrc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3godqlbzn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aggyakuf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3czsgtqne.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qkccvvdd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fkzjevlq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vzqjckms.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3onmjainf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qlzvlgql.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gmgdvrnt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ngmpgsii.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3oehpfxvm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3przwkrqv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ezqjxclk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3gbsrqlap.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tonfmidi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xisucgaz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3svuhzvml.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ljqymcuf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nomevtzj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3urntmjlb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3oqadoghu.html


<!-- 参考信息 -->