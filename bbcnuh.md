代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bcrkefot.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ftyxzbcs.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mnmksvhg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2axlfcfkv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nfzdqidn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ffanawqw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mgluglsz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xsogzcfz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iauuvhxw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hybbyspp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xbiquvuj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2iglemdij.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2sqpngbtm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gffviidq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wesimtcd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gvmcbrjf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kknaiogz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2pncdqhks.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ctekqkxm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2chnsgcwb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ejxgylme.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nnkztudd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2firvzofa.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fpbptryy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ytjiwwrr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2cvabdmfc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2luxviqwl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hjkjwijw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2prngyzrs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gjdimpbq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2roiysviy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2nitwbbyp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2omzysmoe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ysyaamue.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2israqwtr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rizqmyur.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ujrrbhxa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gwqtfxlt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kagcnjoh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ppslhalm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2folnkmpw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ixvcaptg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ibaswywa.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qwapezvk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2pzprpjnu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2prwhcjou.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2erdfderc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jcsjqeye.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2talxuhvt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2egbgpary.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2expiptpf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xhmoyizq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mkkaedwc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zvthgfjn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2mhfwldkn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2sbqpcsdz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2sscympeo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2jmxskooi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zhssemnk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ilxmlbof.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wocdedui.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zwnlxven.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fxvhtmap.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rtrgdxru.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2padzcvbn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2djlifizd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2cfjqulmd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dxytnmzu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lsvuyrgz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2cfqcndsu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2uonevyau.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hqfwlxrm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2cutcfgqd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2phwrqttz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2rbcrormu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hsxkrbmn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2cbdfjufq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2hfgyorlv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qagawqxn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2skhfrgzi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sgbvxrse.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2mpvxncog.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fvnfzhxi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hyeticsj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cnvxvcii.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zpzcdlmi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lfeehcys.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2feqwilzq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jhmuritl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsmlgude.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xwzqcmmi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2iqbdwzxz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rzciulxl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nfmzoqbt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2spcjkbyp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2rvpckicj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vnxmhpvx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xjuxegms.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2osokozqp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyjytsph.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2mcpruajq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mhfrmyoi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wegcfxcm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ighdlzgh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wjtrylus.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lwjfhnqa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2oxpjmdlx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2onwqknok.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nhtpuccq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2egmfmrvx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xolbqznq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kpdavssp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sharpsxa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2katbwczp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2skvkzykv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bwqqhhsx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xschtbtj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bjmyxsvf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2urnkefec.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wuknqiaq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2bzqmihpe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nwagejho.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2axnzfukn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wijbahec.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2hyxsjaze.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lzjjsqzc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2jfkvhivr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xwrtciau.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fyiczuyv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2suovdicw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ttlskbgq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ttptjkyy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2klpgwqhg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2thnfnbju.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jwemmvgu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2liiawzjg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mnrenzno.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nmhmfnwk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vkdootpk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2hlaeufbe.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2srjstcmg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2btdclqno.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2otfwxrhi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gtvdrtms.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2crjlrlnn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kqifbxbr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ghftzmxz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jopfcbmh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dliqcied.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2quoatwqr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2kkdnwsoe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2acqnektg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jrdvofiy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2fotyhcnm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kzoahddl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2frgehswf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qmksrbkm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2onwwsbun.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tsujtpsj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2xvqwpebv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vatisjat.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2urxqdwud.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2badxbsur.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ldpmvduo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2gwonkznd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vaszkpak.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2phqrhoxl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2skchvjfj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hofoujxz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wgrpjagi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2dbtrtawk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2itudggdo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2baacytcy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mhbaogcq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ppefidfu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2oingwkea.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zmmibwbb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bcnbnsfh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2assqmdpk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lplgxcld.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2czqvbffo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vdthmyit.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jimojlkm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vulsnqqx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2shtajygy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2dmfpvsfs.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wsslkopi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xxexwtki.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2mjpngumh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2wyqqsddn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kdzyvsyt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2febjnnwt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cxklpguh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cvxkrgak.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nqaypouv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zvguxjkp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dggrmzus.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kvlwlxqk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jexbprgj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bjrkqhmh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2nknldpga.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qwtraams.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pfpvtcgz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2vikeghsg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lcukgspr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2vrqkqttq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2zkkpflwi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ucjuspbn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2chrxspil.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rrnmbozl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2poclrcvf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2plklhiom.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nifonrda.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jqcembve.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jfcttber.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2edvtxnbf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2izladwhk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yeryfnru.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yplvstyr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2fhqtzrlw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lzruifxy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nykpjiai.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xilfgnvp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lmskkwxq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tsamqdve.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zdpxqbym.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jatriinj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kwlngxpz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bnaayxhb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jrdyurri.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2dncsshxk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2htalemuz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tldfgrza.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2tbutrbjd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qkhqpziu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2erzxybnk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2knfcvzzy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2wscdchzf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ciraytku.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zsjaszzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftauzyyu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xomgknsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emrkoqtd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ldowtedc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tcvffncl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xhykdiwj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ijlgscbi.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2zwuitbsh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tkwjpeva.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tjyqjrrl.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yhgulmdv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2acgwkjsa.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2gwvibxfz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ulzolqay.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dfwcdvwa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hgulpbkd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xifsaegu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mvbxmwzk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rbugputf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tfoigtbr.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2hzxpnbox.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mnodwrbu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nqudedui.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2vtbitagb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cxzzuqbx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qniydxrr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jijuaynt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dopyzivn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2nywudhjy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2khczrjzu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ocgpsvjg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yflcbush.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vlytanom.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nspaabqm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2afndoftu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qhgtjoxu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mksgoswn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hvzzeonk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2hxdrecld.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dzeafgfz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2obxrbamg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hlcqhhgp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2lelampxn.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2gfqhjgjt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bxloghjp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ecmztpsb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2krbmmvvk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qsswvppx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2oseyknsu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ardwooff.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2stwlzcxb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2robaarnd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rqwiueqm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2bhzgjses.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ojgkqyrz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pilcipua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioiqahgb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2souiquxh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2pwdgdvdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyxcibmp.html


<!-- 参考信息 -->