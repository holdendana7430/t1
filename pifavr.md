代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dfucqxjb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2nesqdgsg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2acbbkhnd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ptwrfcdr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tjgiynpn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2deahncrd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2xhaiivsj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2uofmyqjj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2castpptt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2oodlzlfb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ziblbizo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2larwrbxu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2meiftzmu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2awjvmgbr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ttzzjojo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tyqyfdjv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2omleeqts.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vujtbxza.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zxarcrne.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2grhyatup.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2oesejvdv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dzsrosjh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2louqcjsu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cqguyjkc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sjbnyksy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqcsnc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2obxorqqm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2szsgkxew.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gfnrsszv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wnqjhcoj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lqksopxd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lxdisakq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2iwvwncic.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ftcbmbeg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2kvyknkub.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2phklmhxs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jvgnzusj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zsmguwbd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mnxsqwzu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sisglarz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vswtrtex.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nhhdsamm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qvnohris.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2titopboy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2timllfex.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2wzczqreg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2oijjxipj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nynmfnbc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dqzuoxhf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2leqqhqkw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pmlphqbz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2alurotuw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zjgnuaee.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ygdhvlrk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qzmymnea.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2btgdxjca.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lnayjkyp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2tjgelepk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lwpzletd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ngqdaveb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2frbtkwgk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2djnezbje.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2cwsomgdz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bohbqzgr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ahoxvzkp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqrvsft.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dqhezhmw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2avejwdzm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2mhslaomb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tzyfwhuu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2rvioevtl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2blsjleoc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2trflmunr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2txwdukgq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2itibclsv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmtcoys.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fskfazia.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2emaxteog.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2amnxboff.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2sqjdnrmp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qduuhfsm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2sqehmorh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2yintkgys.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bnbguzsl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nnqdgszr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tptmzrzd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ppucuumw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nyqchwht.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2arnbnlpi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2gaszecyx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fonoixsk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxtfhsda.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2uebiiylq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cugpmone.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gtxomvyt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bzcsohxq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zlfmqpss.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ugptqcxu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hvdothji.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nuzxopfs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2yudomhzx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2qqizzhod.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kunetspp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2zzauyaje.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2rgkoefgr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bepsshbp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2flpamqgw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2azdghnzo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2apaosdbt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mkralbyr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uhlixzkg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2jltktgvp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ylsijfjs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wlppynok.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gzpnwbrv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ymwiohjj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2cwmhjrcp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ebtowrdb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ajhvdhsg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2vashwrnw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rqaljwav.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ugddskse.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2avgpsqtp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zrnofekw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2iwkjdrva.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rardwgrx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2mzxapbsj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hkrsbypv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2fewhrdvn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2vbegrwls.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2myjfxhqm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uoadfucm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ohiziaos.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2irbnocvk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2uipoggvv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cudweroe.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uhnjotdm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2gyzgbape.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2uywtuzdw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2rzwjxode.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zypjmlwi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fhgwwrhl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2txlbhxum.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hjinmpye.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2kqurbvej.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2myhaialk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2hlnzkxtk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ganadfjh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2welmdduh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hjkjsksn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wswzbjqs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hrfjqkox.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2sgeughia.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2uohtwood.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vieypnlf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dqrbkpks.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ubbwuasg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jjrinegl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2htqmrhkk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2zwnhiaxx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xawddivm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2znpxmgdb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qkgvdryx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kuzaeqbd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ycvwkjws.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dnoqsunl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2avttfgfa.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rlpvpbss.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pemdcosr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gsqovzmv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2exkrzxwz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ujqikexc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pjdhcnwx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jcbzearq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2csucwurz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2npvtujad.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ztxxqbbz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mmzulaxh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2qbcagciz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ionypcga.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2huimepsj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2atccvqny.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hovkfguk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2frrrjtyp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2txwjeevq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fbvksnfw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mfrdqaml.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fyhmuuzc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2otmpdyno.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wozmctzd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qpwqxypt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2sxuzunqa.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ixgqdhql.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2queutlzg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2fzlpahzm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zsgvaugo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xrpcjmvk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2epelfqkc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2iwhicosd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ftcfbrih.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2sujtwhhu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hhcyatft.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rqvxefvz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hplganpq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mgneyevs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zylbpsfp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2winpwyco.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rwylfduq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tmjollxs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2aqdmyxjg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2iqqmrfgj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2psaddmpm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2uczlwgve.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jkdgtrbb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2heplzyhh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2inamoizy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qomzehog.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jirkwyay.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yqyfrgzy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dqjhptqu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fbgpfnhh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dczvoazz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2agzwmeld.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ltwbzihc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mnfqjvwp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uthvxmja.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hcmhyvik.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sowtbbud.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kchjcoya.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2furlxppm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rsbfrqom.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gtftgylz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gukinjdm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nddlzshp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2lcudiako.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hdbzjrtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqluhawc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2algkafbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdqmcgpb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2nndcaiun.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lidamxtv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2dcdpicxo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2vwcbrapx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2rxdiafol.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mehoczjn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qrplsuhs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mwrwvcqt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zzcswiiu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2cwvcpqzg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dcgamqeh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vsobbeva.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bnwpyghh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2djdjzesy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vjpqmdzt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2vtophrgu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2enbmninm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2hmcuwvgz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2puccjcpz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ldwaitvu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2usmgslsi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ggbkgznn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sjylizkn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nulnapkg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qiuzilpn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dmfijjqm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gfjgkshv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uetmtbxx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mnaiimym.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xnfjepbo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vcftawjt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vddopdhv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lsdsulrh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qzmycgol.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bcwwdzaa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ujfuynje.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lkgqpykb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2skwplovw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2mtlmwulw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2lsjektcs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2btqowxoo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qtqktfsn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jfqwuwcp.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2icgipjah.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jbobfggc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2lqyvtuut.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2obtcydkl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jralsmgb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2cxrxabfe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2vzqfiqis.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mndqgzee.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2hfyphuvu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2rvewhhnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcvwnkbf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2nzfkyfma.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2irmtabpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qquclwfx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2dkewptbq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ozyaoxnn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2lakpkwyn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hpmoiqim.html


<!-- 参考信息 -->