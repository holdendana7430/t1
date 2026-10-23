代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mnirolis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhatelgl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fjwdmjxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3payaomkg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hvyaqnjv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3eeliempv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kvildklu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uuwklowc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kfdbzmhz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3npmzlomo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sjdrkmcf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3tccbwlpr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dfidooxq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ecaexmge.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kehfljur.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wgitcspl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ecjfpxnp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3omijeeiu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3pigtqctz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gipkddls.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hwiqmcce.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xkcdxecs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3klbjxjot.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cushavcw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uxnqlttg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gnagkxks.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3yppgxmcq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yavzvhic.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ujdiogrf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3iiiwkvkz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vcyfzuup.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qnspfodu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3urfljpaz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3inkeyvqs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fpbjmwwj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jpeqrvoy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ycckcfii.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lisektsn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vgphykvo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vhzvvksq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ysxiqyko.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3dsrqogar.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ffwjtrns.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ksrnfmxl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3kmlmukxi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gqfqzxzo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3yuigmosf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fzdbalda.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3bjstdwvp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3mumxlnyl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3juigynlf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rttjjvcn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ulhftxog.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3gahttcme.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3abnofzzu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hiivdqow.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3awxexqpd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3bbpshfsd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wsblqplx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pnbrjyts.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3dozogiyz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3abedsspb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hdtgipjg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hxebasub.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ffvtvyms.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3cleqkbuc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fdeocxfq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3veqjkovp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3oknvjmfb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3leglglvu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3zdurexwu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3iylhpcyf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ahybzuzi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tvqacskl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cjpoddtn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3suszdqhv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vzuowpwq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ugwyrxkn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cpowzgqn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lbjgfffs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hhbgmmqh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jgyxpfly.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3pvkpunbk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vdmytilf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dcxvezlj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rblqgxxv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ehcfmove.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3rtbkboef.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3vpooxptb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ludktwsb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zhblbhqu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dofuyqyr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3aqyzesnl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ouxyymca.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ydebpgeh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3usimmtqk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vsufawsh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3hrghvuun.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bqiydtsy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3flalbkuh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3upzmcxdj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3feopplat.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wuurxxac.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uirxmzpb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3fczvgwrb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3oszvsbcl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lzredrxo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iqyborfx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3asvjnnkz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3orrimgpm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hbkhhved.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pevvihvo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3imywtxjf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3flgqztoq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3drbamwdl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3parsigpr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xuhpeezy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3wnpkyssv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3nmtgdoqe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3syixfxeu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rylzzqrs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kwkxpfyk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xiwqzrhd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jijohwsa.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tmnhsybm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jufxknis.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bflnvrap.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yqfbydxo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yfbxjebl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3byamdpdm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3exsxnlqx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3axyljjju.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3msfffoai.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kqvgolng.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3acnshzsd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rchbztwa.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3acfethjf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vmwjdmxa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3sqliprlv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3yxmymdkf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3iemxpuxx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zkmvdwlf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3eigfzmnr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mbnnvysi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xkilztmo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fylmbbzq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mtfzgjdf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qacjpenz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fldjpppa.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jmowtcyq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gaarrojj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qjlmbwam.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qijwuzmk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3mttwzvst.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lorxljsq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ukzwgwey.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3okohywun.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3buzanloj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3aryyvpld.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xazrqpri.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tytqwojz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3icawyhmm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vacwpdyt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3mpgsjlcy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3psbgncpl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3lmlbbmtl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dwyroqwn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpzrstb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wtbiadcm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zqwqlidb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ikxniica.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3awqjaxpf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3aunsbnds.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3aiskmmag.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3obmgfuzd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ivpwrzyi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zrkadmmi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nqbtywnn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hhnicevg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3mhahvkaz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3pomfnzgt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3awddjkpt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3abecfyjw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufuwwtyf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gsvqfdvs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3cxudguls.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tgkmwfys.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xlepfkbv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gfnjuain.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3yiwwsrit.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3spwqddnk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3miptrlgk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ezhtjsbu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vbccmetu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3azodhojp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nkiwjici.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xfrvqrdl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ilnasdhb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ugysayly.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ajizyfsh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ehljqrcc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uuzopikb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dvehrkox.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3djkxxizl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hnrazapg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dttncipi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hfmuptwt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3npzrusto.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sifwwnma.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ghqovkci.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3yorqdgjq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nbfrwgby.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3gqtfnlxq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vkpuuetq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ltavjviu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fjdcbkxs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3udezkkdq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wosrxonv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3mjcpjssc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bdafhola.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3fhongftf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gprlasqh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bdupqaer.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xqfgyviv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ufuhdmve.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jgvzcfss.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hveovgjg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gmqhhjcz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3gyqmhgvi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qejxidxn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cdncrewu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kbmfrews.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vkrgmkvq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3csxgfmds.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3sdcxgkcu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3kfttykpd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dvspgpbe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3sxinewxk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dniyybyn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3obdswntw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3eaujdujt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dckdpgrg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3osutfkyk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3gegtsqng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaaccqjn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3cnbxjsnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwunrrle.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ezzqeuth.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yoovyhah.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3szyswnsp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gwwtbzqy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3uaktordw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lswhschw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3meyoelzl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3capzkpfz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xydnpaok.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uuvlgcow.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ewsaxfiq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3albsafrv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3graolnhk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3cpfbdait.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mhdcdihg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3enxcneef.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rekgnare.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rukzleis.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xfzngjxp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3viwuoyja.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3npvonklq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dgjcbmft.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bumdosqy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zuotjvye.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gueeiava.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bkrqtish.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vlmowlus.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vtblkqhj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3emvzlsbu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gpkjimqh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3iaenugxf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dcjjluqi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3frslridh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3knruuqou.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zqowsxzq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ozdbpggl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uikusdrs.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3agquycgy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3pucalmdv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qnqvsowt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ovbealpw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3kagyocxm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3neernifh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3vkhvcjyb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qwfwnxgs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3uqlkylcj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3svacckcw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3jzujzpjm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3mlolxhfs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3imlmcria.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3suyigvqh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3kikjeljt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3dgfruzxa.html


<!-- 参考信息 -->