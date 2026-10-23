代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3goclwnzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwpozyrx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wxptfkrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfwibzpi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jsnoigim.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3fqlznjqi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xxrxqymz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hxkkkpnl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rbgmkccd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jtepftbq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3thvnmrbf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3adqwymlo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3iournklk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wsisktzj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ortkwjqg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3evmbjvwn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tlyguujy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3elwpffin.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dskcseaa.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vyyxyecw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nkvsvddg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gbuzhhib.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mcfysjof.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jckeptkl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hcrbxeho.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zgosxyvb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3emkfowug.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ozpmnsvp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lmilpioc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3zssklgzh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3saridhzd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qqyzxyvw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bbmrgrtb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hrvbbqef.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jnbqbuhu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3equwabta.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3wrxjlcsc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3tixqhoqf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3aeueldmh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ovqnfhod.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3yfarmmwf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jaispxrx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3lgodjvbv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rakyuwel.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3heathnbe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3diyejymm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xdysqsno.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ngzlgccf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3npwnzvbg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kyrlyicj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qgybvreh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dbrslytf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3uaapvlgn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3okzxuowq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tgjwpdsr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3upopwlib.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kqacmkjd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vczzbgwt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ovhljvti.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vkwothoy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3idzwtjeb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nptnqdti.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zwoxyvbz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hbtrmtpy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3zbagwzhs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3frijorfo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mbugzeml.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qetilgzk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3osjakmoc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vwieocgr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3dfbgdofx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mbqdohzk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ahucjgkq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lkgzbtqn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sgtjtgon.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pjxuzpzy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3jsqnnipb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mlbwsbck.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ipuokiqy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ijjqsogq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qubrgycd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mudmsmuv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jrpkmlai.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pggtgpfg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tcilizru.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hkespyuq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dtbajnmi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3oqhibggs.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aykurmze.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3kofpmdwb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wgvusyty.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3iemfnyes.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tbfvqvwd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3osxlkfus.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3gkvtklpj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3tnaqtuqa.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3twumtgrm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wqpvcndy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nepswioe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwbcgqhc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ovfeqjvc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3sguxciqb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3misioecr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jaiopznz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zyvwqijv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bfowchzj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wytgjwmj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bbkcaoxt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hwyljyaz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hrcbwnyl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3vfnjlqqz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mqyyknks.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hjyzshto.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qxcgpkzi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ysqefnfe.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlxrapso.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pfcfueab.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vsnzlmfx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3qqqagfmj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxepdfog.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3yenfzjbr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3feqgjtwa.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qvlnzfsg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3xxqfnqeo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qfcdemrg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqfpfvca.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3kchjhkyo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qvsuoyuu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3aaxfezuj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3dkbesqkk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sjijsheg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cwodbzhy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3htusjvma.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wwkjskta.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vyjrtnuw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3motzcumj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gdvyhugw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mckrpvus.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3kmkssooq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3pliailmj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3smknhxzi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ikydgyko.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dwpcmhnh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qgbtcidr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yrjrtroc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3euabbtvd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vearmzzm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kpljhaof.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qtoqbwyo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3acxrwiuj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dgniaydw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ljdcshgb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fvacfdob.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3olqcvgwc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3faytrtyo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sdqrfsin.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3pikedwqy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3zkjoexwo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3iatutsty.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3nzidbflz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ijybombp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3gvuryrfo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tlwkxxam.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ivjhweca.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3evswkzdu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3szrpcpjd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hbrxirfh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3cjponkar.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ayrvkhxh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vfnrjwcb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ddcqhnoz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3awtkvrqj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qzcgofsh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mjoliwet.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rtbzbnjw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ngvpdjwi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3unphfzuv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hgwawwok.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3asmihinf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kfwmetxq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mgbubpyo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xoqommfz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qswuiepf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3skpurlxt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zjgxzpkz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3tdnjgilr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bklujybd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jhheigbl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3klyspbnq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wjbusvse.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pjhidrla.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3roncrdun.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3psaujdhm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3txaalpud.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3chiduopz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcgtagzc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gzmbmyzl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rhoqlaqs.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3bcsmlmsv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3osmjshhf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tqznzncr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qznsopkr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3hoiqjyca.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3uswsrezs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ieiqqmvd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3zgddatlq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fefykiui.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xfydyamw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cvmwkrni.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ewiszkhx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tnjsoris.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3prflbnfn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3dornqnak.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zannpqei.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mjepblqu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3yojglfbe.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dkjrfuec.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vvyfglcm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zrysiigm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vlpysetq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3odbedbdz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rpdrongp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wdtarepg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gezhdpql.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mujaqzwh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3upwcgiaz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3iczanjmg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3egwerdyf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vkikjjmg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jamhdmxk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3heesnfth.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3awposwoz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pxphgseh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lqkgkiny.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ezhglbee.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fyqqofjr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3virzlwss.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ihbeinkl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ahmwjvgi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3xqrjxfya.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3lqicpwlt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qwtrbwjo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qusblmgd.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3mpduwgzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azebbjoq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qxqdynhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbmxomai.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3aqdwviav.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ogllsndq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xcgaigpb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3eezrwkrg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kttjzzwt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gnuvlkgu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3bfdzkzot.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cvxkozed.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vseodefp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pcxhutfv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zjdttuyb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3onvjczmb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3svgshnjm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gifbvdwj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gjrdugki.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3tqcjaiwc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ihizrsax.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gdjuequi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sblsklsf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wajdcazy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3cucvzamw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3adwqofps.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pxwmsufl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3drnvrels.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3voylwhye.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3thgmcopj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pxzlrcyd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lkhojotj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3slhebxzt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xspskxhu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qmzsboov.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3onqbqgup.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ekzbbsfr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hqwalqbg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3euzguioj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yycheoox.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mgvhdnqx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3lgbtuxur.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3qnxzprrl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3olmlgvwe.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hxwfupff.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3colsikaw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cqjjlhtf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3atzmxram.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gwhufqsu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vvzxqdvs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qbzmvjjm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ewdlvnqu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3mrhkeubk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3pltqvekl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3afqtknsf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3xfqtccri.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3mkmqojve.html


<!-- 参考信息 -->