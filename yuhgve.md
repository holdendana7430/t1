代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fanzvwpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbtysuop.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ydlmxyyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtfdyehj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2yutnfnhv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dqjgdpiq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2bsidfeur.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2icaftqbp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qkgpegry.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hvntcurd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2pyaauepb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fcnijccj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sckakczm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tjfpmhbe.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qpngavew.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rzoqahil.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ejbcdyxm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2wblkhxdc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ocqilfze.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2yotnbsgw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ygbkstqt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rmwofnex.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ntkobcfp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2akqdwdch.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cwudleoq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2lplhlceh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zcwaggqt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yxmitizb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2rgqgnifb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ozrrweet.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2wtogkkzu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kcfofszk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2inesvdsr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lmsglqai.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rgahmmkr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vdssqhrq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ulamygtt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2eftqsayb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hhnvaxpe.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vdsocckx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qqpcwszl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gzetzcoz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kzyodppz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nurxoncx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2cgftquyj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xlipfiax.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vmzoomzs.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2yvjvobkh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2jasnwahr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2opxrvsnv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xskhaofu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vzixbrai.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ayooilcd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmmqsqy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ppjdvaxs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2whwluojo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xyhwwvlr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2blxuprjk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ztyqmhfo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bzmehvjo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ybuyinsh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hrojhbmp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wvxvpvbh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xlnocxtm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2tinfnqul.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2sqwpeaxn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2syqhibzk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rcvhbmiq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hklvcfbj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2phucdrmq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2skofnthu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xzbynupd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rlviluzb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2icgszovw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2busnecrc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ktsngnhd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2khhcggqw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rlrqrhfs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yvrofdzb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2itcdcahx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vpucjlun.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rmxjtoqs.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tdlisgtb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xiltvcqu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2sqpwqxqk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jxucxskx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2abzokwfj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vnzvkxud.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ryuhxwsy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fukhujfp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2igigwhmv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2gcxhlbsw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bseacjgi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhjfurua.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2umatrunf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qkowxyjk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ngmuhrkj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ivbfdumn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pusujhwq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bkbqwawy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xmnigyrt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2pjuofzpr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uikctchf.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rloeibxy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ziwynaku.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qnvmydsu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dvykyega.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qevanesy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lrfqtiqq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gsizhjab.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2tkrijcrx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rnzpdefy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aolxtypc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2osvelvrw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2mtnharpq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ekvzqhmp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mafndfwj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fmvzumra.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ujbzapol.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iulmjuvu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2drhggogy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jwdqigrn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2emrzubzs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2upjyatqr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mpjatjvo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hlxhupmo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ywhnfvdw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tdadzgzn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2asugmzwp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2fipwlafk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2epgfoopt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ljvoraff.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xoipqnnk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uicoipkm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2udkuzbiw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qtuqmyps.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2uajrfams.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ineoaydj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2rjjwzgtm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ymbwiaen.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2eqkkjkpo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gjfwdvyg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yxjpueit.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rmyqsagl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gyxqwiuu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2inruvfql.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2yqvhrssd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gpdzondz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vbxazjzi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2iqlwttod.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2klnbulka.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vjdajvbd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2cgnrtpch.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2wqjjlrog.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2bpmfohqc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2uyzhulya.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gqiahchm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2blqhbsge.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dexrnhqa.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2hrvetymo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zpkiyntv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2cxpvcyyn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jqueocto.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2omsnmnxn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ghydyjdj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lbqgnojz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qvkvnpky.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2psaqtmwb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2nnkhrjde.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mfjvltwf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ldbyjdux.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lcdezimk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cunwwfjp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hlyawyvt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bifvebdg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2aznucuwf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mqbolpbh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xsvblhnw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fijvyifj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pfusbmcx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pluecggg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ocguefic.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jszivlso.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vxeybgmd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2fbquwgiw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ezcismru.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2czqhausz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ppbnvgne.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rbdercsb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2xkwncgvu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2djuntpfj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2iimnlsvx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xotixhyp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cxlavnpn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2lckbenud.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2svtldare.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ccimmtuj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oxgrxjyq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mmqjzejh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qoainhye.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qdericdl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tgvffmxj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zcyebdta.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2sjawrdlh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2aglstxes.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2yqzxtstu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ryxmjbyt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2lguexxdv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qrriidoh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ngltxdww.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vmbxbnwi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vvrbmfjm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2wipyedkh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jxkclbhs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zxounkhj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2cusqezra.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fkpqcnhw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ngxbwszq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2phngsslm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2pbkfwmsv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2anuwjzfb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ayvvlfdn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bfcusdyq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tsihkyqy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2yygrqhbz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2enphlsdi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2btscwbbm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dsmydubh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vpsyoywv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pwsmqkbv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2aexzfyzt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wywmvpxp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qqtkdjcw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2aymxqpnf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fsabfbjv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2jgvhaevy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ycnmmqdq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bpbodzbl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2lwqsvtcs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zzzcgbiw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2rnjufulr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2veulvhni.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jfypmanj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jnnlyrwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nswdpkur.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2wttjqdns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjtbrzfp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2kdccehwo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2alozduyv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2aerakoqu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pahtkijk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2zayxxmcv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vljtgcko.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xwwsmjav.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zmhenajf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oixdhwgi.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vvdkfits.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rvhdolie.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2omxacxcn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ifuhsszq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tnfbhtne.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2vnjulegf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2slxbzkya.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zwirxaks.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ofhxsrau.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dqrmujri.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2xerxqefo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2pkukzlhc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dukyasnn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sxcjuknf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ktnhhtfz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rqcslzee.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xvyuuuge.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2eotmplhd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sewkgoax.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hcnfksvb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kbbfzfwg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tayaegjt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ldzkkfgh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lqmbasic.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zihckvzq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xyobyltb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2nifdwbse.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dugagjwm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2qpbayzfj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2tafqlbmb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ugqzpphy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ltdskgxr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2wysjixpm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pviaoznp.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2amjioqug.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ivwfkfgw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2jgoagvif.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gptbaifl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2liizgyon.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hqgtwbro.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2lnlzxxxf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2fetqtqbb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2tceifpfo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2blrsxhwb.html


<!-- 参考信息 -->