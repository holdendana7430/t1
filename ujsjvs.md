代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2horhzvvc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ziupsdcg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vdxyeqil.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kqrmctsh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qnkbnxox.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gsrpswal.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pxxivdvf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ytjpwlxw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2rwbzvkbh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ordqhgiw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lfxthops.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gafokihg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2cedjbkub.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gkzllgto.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fgoxntlk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tyovinmt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bbgnerlg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2heuubzuh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ssltmhsw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydpdyxfw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2uxkelddi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rofptjlf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2evkaamgh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xskhagln.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2nkurqebx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2brwzbbqj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lqmnhymj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2loyysrea.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2uqbnvlha.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2aidcqaug.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ougzwtgf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lpifrcdr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fhypcdsc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ikdwqrmd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hwszlavt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2bjzuifzq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2suovimkd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xhufdmxx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rigwxeka.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2wasfrqaq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ykykhcss.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jzowegui.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zvxejznl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dddnfioy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dhobuflx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gqqsqkxk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2uznngqds.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nbuphegl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rveuuqor.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zhkqosdk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wrvpfyof.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bzdgnxxt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pgdzlozo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dhefogsn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bvbaoaba.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rydvdqlf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lglkdlho.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2znhyieiq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jwdtarqj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2yeaebnxe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jnhjivuz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2svxbulve.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rgyafvro.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nfkknvtk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2oqmwxfjd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2alowcsmq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hpiddsht.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qonijege.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rlpabcgf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2umpusqgg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2iorchvza.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mraauhtn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bloaytsn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mqbdjhoe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jxnprpve.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpmkwwc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vnhkyhsk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ascexmvi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fgzjynph.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxgfaihb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rdfgzdue.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2iurmxxcu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2kktylcrb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kpefoghl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mgvdmbpi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qfgsomoh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2rnjaxqch.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2guuxagql.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rhasbgev.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ofaiplsu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tklndzyr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pchnkukx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mtwtvyeg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2aevjmoin.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2lvkuzeil.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jutwpywc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jomcqcyg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2udkjlhcp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2oojzcovs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sejikbhm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xlkrisqa.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2blurtioj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2wquqcmjq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2syqrqzsw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lobrstxk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wyzkugrs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jzjpseyr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2afkqoulf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cwrrhbhm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2vanvymyw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2evjnzdni.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2skiybbep.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2biqqmrsn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2oezdmwob.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2faitjiwt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cdejxwtd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2givftcdj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pazpagdl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2gatxtdml.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ufoshwpn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wfmrbxvk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2inpyaeha.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zaasabwl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qhbnajak.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pmnlooxh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yphyteql.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2hrhqtyra.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ycpdbuzi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2qdujazwi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2nibkyunk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2usabluyj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wilddtni.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gmeqydlj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2eyrlflfp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2imnzcvfw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gmskdlwh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zdrwtoyp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lthausjy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lrlcpuln.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xwtvbbac.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kydnbbog.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yhdydxgk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2edtgehkr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2oyzqaree.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dqsdaapm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lxnfqldn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2cufcezmw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ujfcypnh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ltqwndji.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wsxvvivd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bbgawkaa.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2cwitdzpt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wjlzlbui.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rleuzmuf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2uaonlbhg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2kyezswsf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2krxxyjwj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mcihtcxp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zdqtltxp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lczjqpio.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2hnszpaea.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xtnqryxw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2dlnlgjay.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ntilyosh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mtouahcq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2iypvxnrb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2dmipvmkc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2yffxrchs.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2abircard.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2uvkhngaf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ointubmt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cwbseitq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xnjbswre.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pfbadwaa.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2pqzempey.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gfscioro.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vxjahsfb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rhlldjru.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ynlbfngk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bojvvabc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ktjxmabs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ayzhcjqm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxjyrtbv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mxoaotcv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2unyoaiuf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jvzfewgd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ufyvcerc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kmwaieqr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lrwayiqh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2orisdenl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aikueqym.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xkcagjhe.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fovakzut.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ufelvuru.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mjfkhanm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2nqeajsbk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2rzfaqvwe.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rjnkwymf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2skkaobrm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2earqdwzl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cuatcpdo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hzfypjmu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rooujmqn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jhiquufc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rfwfbmcj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2uwnfeyoy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iagsjtof.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hwohicqe.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jthuchoo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bnyoiphb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2covzsiqs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2smwastiu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ozxsuzdq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vdkxedah.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2enhqmxim.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kkrjfrxd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cyihakkw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hkzsskxb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2boooyjen.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ndolvlip.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2aptnfypc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rhffxnzp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qzwspdxe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjobtkp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xcmccudi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bwsvplmv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2molvbekv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tprukvry.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vysfbzdw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2bhtlzzha.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2jubxyorw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2exfumemb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lzrngfai.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2haluuntv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ovdprito.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wrvpgwkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgsyvrxb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2gsyjjpsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fikcsuye.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cpvytzzc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2plrlwkcn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2pdltmmyw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2pjtrfjra.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ozktpvqb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2etwucghx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2prlbsffv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gryxrtak.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ljddnprb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2uywyjisg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dcbhhucm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2swcdctse.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2yublgitv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2cthtflap.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2sflfpqxg.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2zrfjuibn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ffusavmm.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jhrqyzvw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uynllzlh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nvmscpsn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2urdasvnm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2nomrtlze.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zfcgbroe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2moxqqosc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rmcwtezn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2bdhojwym.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nvrbtxdx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bmmgqmyj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nzbkgcvv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hncrzitx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rutrxpsj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ipmlendv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iphomwdo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jrvotulw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tsylinvf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2uoifawau.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ijenyuzp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ieqsaqow.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2zdasacff.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xymzciae.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vzvrvlux.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2pjosmdmp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pwszykqc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zcwgiwnu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rviuubgk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2qvhttavy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hboghykl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2efksdpyg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wunawvbj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2pvcghrkk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2emxdjkxq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2fomphmtt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2negnrygz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncmhyzim.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2sibxcyxw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2qlzrepns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inacdzfr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2syigwhkd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rtzldufx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gguvaijt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jglgfjty.html


<!-- 参考信息 -->