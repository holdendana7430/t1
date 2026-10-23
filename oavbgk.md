代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tqjtbmzx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xqtytgdh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ehpnxdbx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fmmowwou.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ciqocbxl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wcxjtvrj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zbsazmor.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xwcpzvqr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3kaatehiv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tgovnkkc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3yeyddhis.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ktzjpbue.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hnhslnjy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3utywzrfx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ejnubtuu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wkqlrtww.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3npqvfomm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnnlrjxo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rkumwqej.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3qtajmnlc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3arvoreuu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mapnnoqs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3cmphrnfs.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qmxcxhzz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ezqzwrnt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jxdcwkog.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3komxtuyq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3qysmrspj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3uqmpnlft.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3odqqowuw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dhujvero.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3auirpezr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tbiyjxjc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjmtjbot.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3nwdyorqc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bahvgtpn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qjpwyjbu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3aghxlleq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3rhcctteg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lngjhlqe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lopybgtk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rprlgsaj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3uhlrdoea.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3syhtwtcp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qtazvaed.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3cksmulpm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pikthgso.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3lmiwudym.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xxzmzvvo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wnwjobzc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3naqpizky.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bcvjpbhv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zalogboz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hnxcdjha.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vctiyrxt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pwjookvl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fxsnpscd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3nrmrjgcx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vqhqpefd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hqlafamx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jcvnnpal.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tdpahrau.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3huqnbetr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3pxnccqjh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3uuqgmcvt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tbdqsrsa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3chphjbdq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3qognvjeh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3egrfcpsz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dfyywqqd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3iexgseow.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3eolbjvis.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3aqqbmipb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3twkvmnkl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3knotxfmg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqhvjcc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jzaevbcl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ikaewyjv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3lptjcuob.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xjjulnpv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fhekckon.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rybthpyy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3lnbcfskv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ghrmkopl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tzrtluxu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpsvmwzq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3avbivvzz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hkszqlko.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fqegdblv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xaiiowka.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ecycdafm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xxrxvorz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3bgizmrif.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ygohpeft.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3afqtdwxt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ddxocuir.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zjboyist.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3iwvpncnp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tpmdewcf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dcggxlel.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lycwsogi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3bkxdsswh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3agrazwhj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ugamqpwq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ibcazfgd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3trohgubg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgetwgph.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wxaqmyqc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uujoftxo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3fowxbtkp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3vcsnmsjj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ikcbvkdr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3fgubdjqh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ptmwngov.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3eydmkkvi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3gjrvevnt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lrhiysaw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bircvyff.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3skawytte.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3hqeuvmua.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3prgpdnor.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qtzlpykq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ehhpstep.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zgkaxkks.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3maookoli.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qwyvubob.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mrejasgi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gnmvvecn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ckuozfsl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lsnzifzf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ghxhotnn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dsjvaozj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3lvqowped.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zyajafdb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wkvtkzqh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hfnvjvza.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tvcxcrzx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hkefphgp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3lzbcpnad.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rrwpclqb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sxvpdqde.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3tlggxznt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3subaxhyw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dijaovzt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3aadtrfcl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mszgwxop.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jcehhyic.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zytmxgrd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lqwoplxs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3drlvorsi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3eqfqaevd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zgvicgee.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ktcetpao.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3akdvliej.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zfjsyxng.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3iekwckjz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ebwfqwgf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hodfrrnd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rfmnyomp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3wqohpnfj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tetxsvim.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3spoczczp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ztkvaqxu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hmxpinfg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3eayugsou.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3enouchas.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gcyyzmlk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3bkvmsizn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wqdqjpkw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xrukxund.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3mxmjvent.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hfxdmxam.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qebigykx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jiuywyxd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kgahwbdp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ribsnpkd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lxrndtiy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3amfrhbzg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uamlwyps.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ixcuovky.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3aupgwcfn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3fcoflars.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3toeqjyvp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bvzcjwtr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3adgrspsg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3drqwppmp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lvflnivi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3plihpkha.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3iijuirly.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jojidhdt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3tpopozxy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3pksprcah.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xvwgjjsg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pzcofxmi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3bjbdutau.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3qkjzvybj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3enrhfcnd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vmolrxwl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ljmqnsam.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bonxisci.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qkqcetwc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wdfxfkdc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dsrtgjci.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mwmrmbjy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3dalzwoig.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3umkmskhp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hzelteal.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3urwtfcni.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ejhmeowg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3sunshiaj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dvtzhftn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3seoveovt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bifpdbtk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvjeuxe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3zbvxryyq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ghccypok.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nagulhss.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3scfedyvl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3imkkyhuh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iabrtpzd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ykxkqbem.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gnqzcxvn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gcxtfypv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ybnbcuqu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3enyawhsk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jiqxwsif.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3giyhwegm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzjvinbo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jgsnbvtd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3aiuzxlxf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qmeexeln.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3zbvxogfe.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ohgpieeg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3tjlwnmcs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3uxrmffqq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3oznzyryf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfzqzujs.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3hnzzhqss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdeuvmgc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3pacqpxtr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3flanrjkt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3fqrukslg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fmljkdbw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tztlbcgq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hmxzcrrc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pwobetov.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qrtlhgxn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ughskfuz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3czhwpioi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3glubfodi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3bcwocbok.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wzhyjfxz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3lgyxeyzn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mjcqvnzp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3anuhoooe.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rzkqhqje.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rgfmnfbr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mwvorljr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3sbvpzgbo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3pkhfxebv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jndcbrvt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nbbpimrq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3erktwsoj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3opzsvkaz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3btcjruav.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3irzoohwj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3etdbmqnf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fiqzdhpb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ircxaylc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qdbnywmr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kohjrmji.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cpaceqrk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zvsvsklz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hqabvqol.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3fifbqnoo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yvlnpxgm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ovqtfcyj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3owgxzmag.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3idlichhp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rnkhommu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3txynoxpd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3juwdlmgc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qskphbpj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zviwpvef.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ehjzaqip.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ewtjyidm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gusxevqy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3encmwpjj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3gyriyouu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3gzygoanq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3liqxijfj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3wtdzvdlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujwrivmw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3sbarfjoc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3kayqewss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyvrgsvo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3sqdtzgft.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3vcqiafxv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3htmtltvy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3pgheanac.html


<!-- 参考信息 -->