代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yypwzvtt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kifsuvpz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3adrliwec.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3weicbuhb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cimzdyzc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hznpoxwj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qelgexbn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lpconizj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mhxmasoa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qqfkylho.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zzzwiatd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pthjurhk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dbxiesop.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3baoabcfs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yxaoeoqo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wqptzfaw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aqbnqcxh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3shxgpcqb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vicovglu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gnyfcufa.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjepoqju.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xsmjpbjy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3zotsoyev.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfblkkl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fezhrvpn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nxujprot.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3iwomxjfj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xsjfhiaf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zkjjxpun.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3iswrejxl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3avsjuesx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tbmoqyyc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vrrqmnut.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzjpnmf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pnhobzvo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cevtfans.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3artqexxy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ejodbkhg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zxcgluuj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qncnvoip.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3afnorydl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3htyheugx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dlypctfg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xahkbvlv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3okkqzixe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bkhlvxsw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3itpixrbo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gqxpwmxa.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xdvmadaq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zdvzpkug.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pykxolcj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3itzphoiw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hpqyzmvq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3pvlipnoq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3njjuqraw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3yolfvvvq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3npyognjo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xhvdqpxd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3xzngrwqg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nxfalofl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3aattwzcw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rckkileq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3thprtrvi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3itstdfru.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3htpdbidk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3icozvmqp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yyfqrjrk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3unqbhrpn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3acgbiedr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vtaktzcm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qvcbllxp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3efvntxcy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3trxiacus.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jyikptdk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3lkqlcnjv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hhxxlhzq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pbbfapqq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bsegwscs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vdhkzjdj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3scvectpv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zqvhaxra.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wvpflsxb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mocjyace.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3aakufpvb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3domyavkd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vpsflwui.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bujrxfhq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lvshyheu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qnakugwf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3hosudleg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ekxfdsyi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3efmpsrjy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3qmpfbzwg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dnhymrse.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xqwmueef.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqbejjwc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3uccslmtr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wnghjhwe.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3okpzcqzf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fbdgjbcj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3rdginuan.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3orgewtbb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fbhomytv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vkmmioyo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gcfwzsph.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3avjmxohb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gsdbzhod.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rwsnsujm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rkyvimlz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3nhlmwwue.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3absnywte.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gebpsxzc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kjfbkohg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fclfngnt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bihnuaoy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jalgqygl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zbmsepvy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vcukkden.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hqotmdsj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3biujzrnr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wyqymxbn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wuarfxaq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3peutuuxd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3avwedblc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3wpbaosqy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vbkdbtoj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hwdxvcxq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3anqvotln.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ntltrung.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3exqkemhp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xzjfvbbi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3iaxrbuae.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3drjgnxvt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3yfdvfwng.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3prsuxknp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kvserwmd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3agzaxrsy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fnzbbdid.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3dyjvfgwd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3azjqpehs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rkdxehtx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jvuyeaab.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3luoubhqw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fgbcmudc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3koifdueu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bzumvgdq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xvwbbzjx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3qbghfktw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3yuwmedye.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ocanmxco.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hpvhaaco.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3yprcrtgm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3onodhlpj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3shxzhpuf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3myhmhtqp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wemmqzii.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hqvunduk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3pcepdtec.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bvzmxuqw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmccmbt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3jdgnmjsy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3phqdblds.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rixjlrqo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3stajwvhs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hgiwtdrv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qvfprlzr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3uiocithc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3dicbpomx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3opegdyfg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3iwciypmr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3tdunbdwv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwsqvqb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3svuenbsn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pdvbdpsd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rewrdmol.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dzgiijpv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ovmfeaur.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wtrrqlju.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3yseklxjx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tecaixjf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ikghrpez.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3kkbvnxwq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mbitafeo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yrdketbo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lqmjdbnt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hmsyiqok.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qsxbetjn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmtjuxit.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qiizkydn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zylopdsf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3clxmtdbf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pxqvulie.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ilcnlivj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3nrsrqgmr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3akdekmpc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vixpesud.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3uemowypa.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3mlzofcnh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3yxackjbt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xtlkbhkh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xkiphomb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3acgmmapz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tgubnfao.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yhkeuuat.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lswzwlca.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jkiurvyq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gkztbyke.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3kyokhile.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dnkwlmkd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xqfqqiul.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3sqkvsepo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3aujcuzsu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fhvzpbsx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xdmbcstp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3vzqgqmmt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gfjrzvwo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3njzubvmm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3anckngau.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3pywfijxk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mmmcvooa.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3skykpmxx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3joxfuhri.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ltpbtzeb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fftyejtq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rsyzwrgy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3baopsixr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jytnenet.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsvjggfa.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3stnlxbxx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wbqecqjt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kynalmdg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vxkwfeux.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3gmiizfpl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hnsnebbr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3mwakgrkk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3dvkoyuxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sloebzxs.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3yadihpux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlbnypdl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ynohohau.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hkzenfkp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ucqhnuyc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bzzlrkmr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jfqpllul.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3eocwfvvz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3byghnuvr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kizyeqbo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qvaihywl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3dfnuihcn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3tffqwuhq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3jvtxcibj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3sgiujawa.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3iqngokqt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3yhgeadyo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3krzggrrs.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ktvizigl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ztewxvkk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3edlkelxp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xfrvzebb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3vwfktbmg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3edihepll.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dhiexnkw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mqlvqxaf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ehlhmxen.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3qrmjcbty.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mkjzxwjl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3leuhsukt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tkdjdcke.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3heqmhcsb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yqjiibbj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qvkjoljq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3efexaopy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lpinjwjh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3saiugxrp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3jxacazfv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fnjafusl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3fnbpcvpo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ltoreekt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3onbfejcg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3snltlzgh.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3oswxsual.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3idynftgc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fdkmioue.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nfdhfbet.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3pwebbswl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qfrettka.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qfeqdbrq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ijiathng.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3mgwakxpp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gvchjnxj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3swkpzvpz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3lvxaddcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgcvzuvz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3brfwvvgx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ivjxlqee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idklimdw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3jbsbnlmf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3qwzgroan.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3pmnldfzv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3toeytvmz.html


<!-- 参考信息 -->