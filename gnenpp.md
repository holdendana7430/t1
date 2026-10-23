代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ifjcgbbe.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3chjvadif.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3loeswdjz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fuwnnrli.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mifasrgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvqrgqvy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rpouklkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwjyrpgb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jusntylu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jauwvavi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mqvpmggm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rrvwknzo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vzrlxslm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fttdcnii.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bwmhhxaw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rfwailni.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nyrvkmpy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3aenqyuit.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3usibaqum.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jeclelxy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wmaqdjlc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3oehexpnn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3aeoyzykn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lhnqurbw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rlmidrxn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3owmgyjbz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hsuwzrop.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3unzetmpk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xucutixr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ubisxcgl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yqzsgapv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3qzajptjw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nypstrny.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kbvunkne.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3cnkzyqwq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vycbkrqg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vldpzlta.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3evdpcvjz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zxuvuiru.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ogujsxfn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pihlrrjj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lrzbukys.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dpzbtqdn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eotnldtl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jdffscqa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3atdiuink.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3szsofvqo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wqknhxwl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fsqddrll.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zptlibzm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dcakmbme.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xjfjtmzz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tdxaovxq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3sbsjfkzy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3xtimblni.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3roktuuth.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3znrbhxor.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hwgjatyz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bwlllwvr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3lvoaqpsl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jcolwdya.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3smpgklph.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3gjsprves.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ptomljrr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hoxgabqj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fflunqbp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lgutpfgx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wjklcdlo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bmzwrsnl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3avggskgd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ifxrgxzj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jmclljxt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3izgtmmhc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kabyowzy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fgbmxtid.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zdxrlhsg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3swlcckjv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3nameskls.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3uwgsrcxq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jzmyrctr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ropcapiw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3noleigdy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3afvnnagi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3nuygzsny.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3nmktgsnt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kzudnrun.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3enduvxwr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tujfoiwy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ismvczmw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ufpzmlfz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fiyudaie.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3otquhmhn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3apphpnev.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fddvvrky.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gyzzvfao.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cumhwmdq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3oeifamqo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rdztfvmh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3diapelqx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3uwqdtptt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ewmqymsa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jzfbmmxq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3sahkwakk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrizmuay.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ckkyrynd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gzwsgkym.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jwvymrfz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yirnbwky.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xuvunzlt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zukozocg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3deteisvh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mmqtpfem.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ltautsol.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gaubnycf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jvnwftds.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3mffvxpwf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eqkqykpo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3npomxiuy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3apisglcz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3afpvlgvq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wqqoqpji.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3kfeovoex.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3devxjkze.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ovlvbqtb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3lcqxmprg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nofidesu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3tppywtjw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ltbqexxe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3prscgkcw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ylzwduqf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ldltjyjb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jijmnnah.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rumwzkyf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3dazetnhf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pfysltix.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3kpowglbc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tjwvphcq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cnixxedr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mqxrcgal.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwmghjxx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ufsabpgk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yfzinogz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xnemnwhv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hpxvkhsj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3puaoonrm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3asofegvx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3oisxrsmq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cgbqcadk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cnmlgmaq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zjecpeyj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mgekabrg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hiodbhno.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3kvqggxku.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3mimksrez.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nnmkqliz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vfbfgrkb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3xdjboztt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3gmfhpatg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gmtafslw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dpbtyhiq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ijpumprf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3yfqjwwaq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3aezperhl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3hsnqenex.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dkfpqlwj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xaooxwlj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3bubokgrh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3sqdprfzm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3bvpbpuqm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3beazycbh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zvsesxro.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3yncbichp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qpvgzbxs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hocgtpxp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uahrhxal.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3iruvybmc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ugkjxclk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fsbzzmta.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hljrmeas.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3pclkcckv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3edlagujq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3arcdnvbh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3auqtcuqk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3erxpgwou.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yoczwhbz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ssywkqkf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vgtdxbvm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vubzjnzd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kqcfdgoq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gitvlcbh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jamfqwvd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzjktaew.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dlmldvua.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3secfpvos.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dnwjvcwo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yxdwyaej.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qmghjmrk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bwchvmue.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3smbgavyp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vekpdquv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wdqbzsmp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rxpwpueu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wzuwxlfi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3miwsbxbn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3alfcsdpq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gmdxjjsh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hxgpfbvn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3akzovfgz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ftunrnhc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ofmgwrjs.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3usgidbgr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hgstrvan.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3mpajdvmt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3rwyljpxp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3usdqsqai.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lkahjphy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pdtdejdd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pobfqdnh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ikzzrvkz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lfqbrlyo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jyncqeey.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rkqxjgvu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pwiahila.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3voiasnep.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jlnbvjjr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3byeyobih.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lphlmxcp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xipglpib.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ikbzvqbr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kbnxvgnt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3sayfmywj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xbrcvvze.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3awaxuajg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hnfosrag.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xoocispn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3twaqcuji.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ltvlcvqb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cvtzfbky.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gzdrbznq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3dqrggtkh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ysoohfrd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zvjrugrg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3orypcfqf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hpcybqvp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ykvxfxjh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3oedylwrk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kvmvxscp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nvuwshpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pucugdvu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pfbpixgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smvjvwgh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ryydwxkq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3sklpmwcz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lmnmtgxh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3acgsobfd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wpnxmfqy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vczqtmhy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mjmjujei.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3donuydjo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vcsfulpe.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fcojunuf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3enisttbn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ztctrdzl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3pmnmzgut.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nmecveih.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3geonlbqp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3esdvgtzo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3edffmzmw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ovwafggz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vailnzrr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bcepwilk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3frirnwna.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vhqlcvzb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vncirvim.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gadqvaim.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cuffyrgr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cnpablvy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pfsryhis.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3brosujvz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dxvhkgph.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3duzxcoks.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tgdtypjl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3atycsupt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3caqczoyy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dqylgmrh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3swhzxoug.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3zxziyglf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mrhshngo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3gprqozcp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hzczpkyf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3hripkruv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3kaxptwti.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ukbvrgjt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zwwiadpo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gbljyodw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xmntsvxt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dxwermgu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ejiwpqmm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3icktxwnt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zwetsxiz.html


<!-- 参考信息 -->