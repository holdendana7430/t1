代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fmwwepye.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2acdodbbs.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hicychtt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wwdyqttg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kvidxebf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2uiyzawtx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2eiiftuvq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2arscfcna.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gkjohvmk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xwfeodhp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ydlivxyd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lnkfvrtm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kdiorknd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qmulietj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ovmkvjud.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jxlraipw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2thbtbatm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kujdwnqn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vtguuhli.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvhgwfa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qlnwqnhx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jvieanpy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kqsmhutm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kqiksawt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rppqgjtm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2lybsgsqu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2grnzmpxk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lngccgcn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lstdoxjg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2iggozdif.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tlhefycd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zeeclsyt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2sieaibwb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2hazuhpwl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2iyhfbncf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2vxhwpfyw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xicinkyf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vrckttrd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xkybjydt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nhqqxjxq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gyrxcdyv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2eppvsycg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gruvggfh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wbeanexj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ulzzxbgr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jlemxopi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zaibcvok.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2smlvvwef.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2bvaeydsx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2txlkgctf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nixdvteo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xelixtdy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2yusjxcte.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wlskumxm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dwgqcgqa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yfhlpknx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2eficmpxg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cqbxvxbz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kswzckvi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2uwwucyra.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hjzxlnds.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2oyeqhuvj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lukmfvds.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2kseeunhw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kutlvswj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2pxxuvdtb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2snkqwjui.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2cuqzqkiw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ecmhfbtd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vvqueevu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2chviecuz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mqjrkcto.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ccuzdwgt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2knatvwqd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2smdnrhyw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2kezfwjrq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pfkrqbvd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ksejlcgr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dyiblanh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2akwndusg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ggjuslnn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iflypqwo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2itxtogde.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2cdwiiisf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vlnjjwrn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2klnjlmwo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bicocult.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jmvexlfn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2iqudsllt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xbnekeeu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2cildpzpv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xedinfij.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mimnvgvm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vtnjoivx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wxtsfaer.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zuroyddj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2rbtmenqc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rmxfvfqr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zejxuqla.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gpjbiqro.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xycubsfn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jvdbvrud.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2mjjjzrks.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oqdbkmwk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gzrzewvu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2xvizudtv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vthaapxp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mmjvimqs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jgdytmig.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2doykekar.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2zakyeqzy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2oybzyrsd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2jomltvqu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2obyrottt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2eektsaeq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cedqmzfq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lhwoivkx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fswedzib.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kyljajfv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2feppwqjh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pfibwrnb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nxfgcqro.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2psivceba.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2eqwbzzba.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2sddhjwup.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2mktznpws.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2zkulpuwv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pxovirqh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2esysklro.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2sbiidajn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2llkmyqtu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2fddarqmx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ppeqfprk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vtsidhfq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2agyeogoe.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2hwlmquhx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2npqivivm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hyiaoglh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yzciyyna.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2nipaizuc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2lojekgmd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2etazigql.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2rgodfqku.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ftnawkhv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hinqegih.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2morfkwce.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oxtbsrkg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2clssxatd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wiefmhsv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vqoeqzbl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zgxfykqy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2uvvxnpst.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pirnwcci.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vpxneemg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2gjwhfvws.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ubpfbdnm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cdjjpnvc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2iytomirx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hhiufnib.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jaricdiw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2pcyzmxim.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2oweiwllf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2drwpuned.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2smlxmgxj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yxcwgrwc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2itcwsosc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2drjegikm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bvpmnjdw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2vtbpjssk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uyhcampm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2bxrwstsr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zarqufgn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vtmfwvjo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gcwktijm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dxxnclue.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2onxlntiv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2etsmxycj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lymgpfux.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fthvfrhk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ptagwjrl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hixkdfzs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xkopelky.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jahjcxib.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuqaayuf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kzondqve.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2esszwgqc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2esbpbwmu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zhbjziaz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rmlxumid.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bydipaud.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jcvrruep.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2uvlehdpb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ytapypkj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2kjswtrsz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rfyxcaqo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hqltdhwf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gkikehui.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2aaqmdzsy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2krnakahb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oqzczrya.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mmwihklq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vrvnuoxu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cbljvvbw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2psboxzzh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dnpjaznd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cuovhnfd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gxweufvd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yqrxdvwo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ecyeyapn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ogqrweyi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2etdfakcn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2poucbukg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2bzacbjen.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2abpwovwk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2gksnnhfb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ixposhfa.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2btidifzd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pqgrbxqs.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2djlmfqyw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ytqnooes.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2sehhacyu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jynjikwa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2uyvfrvco.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vptzibth.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qoibevfa.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ydsefplx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zqzesupt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2sjtorfng.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2rdtiilyy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zfhxsdrs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ftylixwm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2cxzkdczk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjjsnddx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mggrlbho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvmhyneo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2tvdsavpu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tgxqqyvx.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2lpppsmry.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fliazufa.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jvovafcz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cjgchjef.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zewnmkro.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2eyaxtaix.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tnvipryw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2znlyhzls.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2bnjfhazb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2tbegfujo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ldbnpsst.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2gghhawjf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nbzjtyet.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2msdjpwma.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ngmfipsf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ikourrmt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2amrlnjod.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ulifvtap.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gezbrjyf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xepdqtnp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wasyhzql.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mnwdbfof.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ikkjdgfm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xonhfsgo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2urmkijlw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vnlcpruq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vmxmnsoc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gkhtuqno.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2omxxbsht.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jmrezhql.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oxdxpwbx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gxhuuyah.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2psjklmie.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gqggeavi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ejvdfowh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qbbdmnnp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qtskifqt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wrpqbben.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dodqbvxm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2dzivritx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zoorialp.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hdimfqxg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2awgppnht.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2rcfofisn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mhpjlohz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2scyqujoh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fflzjryp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ymnxlgel.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2nispoybu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2bzohslgu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qifdyvjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmspfkww.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tmxanpax.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2keipwfmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poyrpitw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kvwjyofc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2wdmxxasr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bejvmoit.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2znkntbsw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ipyttnlc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2hwxqrpdo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2npurybkz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2fssytxbx.html


<!-- 参考信息 -->