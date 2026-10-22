代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jliiojox.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vqesnvso.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2iskeshif.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2nwyixypb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2pznytxix.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sgeqseuu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2clviodys.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2tyknfaij.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zvszrgfi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2sblshcpb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bkhoawqs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2kdjwblxu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dhkvkibd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2fxunlecs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xzmixzpe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2kgrtilrx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qyjulmub.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pnlflwan.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2rojqjmun.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ariucgru.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qaeqofha.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2eiiavspi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2fkdpdpim.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2yiahitcm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tqqfqjuz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jjbyzucb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2jdyvltii.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2wpdtmyov.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ubpoiiyg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2bhonabbw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2flghaeiw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wtkqausc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2yvoqrowj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wttacdqr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2khnnrqwq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qgffiqqs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2alpvhkak.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2lumisfwg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vqisoumy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hvgowboy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftbpzcax.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nwapwzrw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ymbctdpy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kvcgjvgu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wfnrqtry.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pmgemhgl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fhouoxtl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tijmdorr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zhlyioar.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vxmyydgh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2yyxgiivj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2choprxfi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hpwghsuu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mxxtmuez.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2kpznpneu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2zktdbxoj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xkyxkcgl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2adynqijo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xdxqtbgg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2liaxhlmi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jhnsnfih.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bfsdcjwe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kwmajojf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbbfrjf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2paemqwwa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2avwrfqmx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2etygcoug.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2yggsujgy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2egcnjfbc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2twexobdb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2dulqhvgi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2fvuxqinr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mfdtaljl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dfahtuid.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wvcnaqfs.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ovbnuxkv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lvyujwzk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2illkhhfi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xfuqvupl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2pfmxeavu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sxezuwty.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2evcnqocl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wfgkkdvi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uxumvzpi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2yphlbexv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kpeodzzr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gmqlpfch.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2meqzgxvk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kfwvmnsn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kyocddnj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2scbkrygf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2etwcwvvn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vnltslyh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nvixcpor.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2afyxwpab.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hpiqflhq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lomxxnmz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2pyfwijss.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ivhiqsyw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lehwjmhb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2dhizalwn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2yqjgktzn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xippinpd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2zjslucju.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2pngmtblm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kpduiago.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2skumhncc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jjdqzqjx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ecmdwsce.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2scgnyjgw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ualknuzr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vrdzwtpm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2okakglnj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ghcbpwwp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2idyaklnp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rtqbgruh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zqdtfnzw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdeziato.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2kkyoybtf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2vrpevimp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2tmfjzgsk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jjhummjv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tomowuvg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ymqcfjwr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2wiymlgol.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ytdgrjzp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2tepgtkpk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xvirkxza.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ywrovfrd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vcyooqpu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fuelkptl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ikxjvymj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fasydouk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2qwrbjjda.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ghmmvnek.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fzrlhgud.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kfhjketb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wmmplzxr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2avpyocxg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hmpjqdtk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zxpkzxiv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gseyxavp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qtlbjyvt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jfwcdgdn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xtnlzvte.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rspmtrnz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2grcuhqtn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vzfcearb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2fqtapali.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ewhviexw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tfpsgzft.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2isdzdbmc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hzwgiewf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2cwrehlfk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zpszcdig.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2eheumnla.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ouegwqcc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ccamihai.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ksbprlra.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gerzzexq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2yvucaszl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rooukinr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2cfguterx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2imvqpzeu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rqmhuqcr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sfjepqrk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bpyagier.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qwsetmjt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2valansnz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ibzlmlyl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2stoovyxs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2daphhiyt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2eoavesgs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ryivzqqp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2vltjjamk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dwwqdznk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zrupxnwa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ztdgwinn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vpmttuya.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2agnnzsia.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mebffzdj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2dhicefrd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tctrmyxm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wzyjykqr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2naktozoa.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2fmjmhbhn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qkxelepl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hatclqby.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lfplmjdi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zgtaufwm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eqtpqnty.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2bdqiciqy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2voqhjyjn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fbxpznvk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ukqibmmu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2evqcdrlj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ftngunek.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2kjnzwkme.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iacfyggp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jybpfsyy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ikqwqspb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lehbkpex.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ltfdvfuh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mrdibbea.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vqyzllto.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rsdgrmrn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wlucifbl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2weiveosn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pzpkcgkt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ouopzsec.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2trfxnmbh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hgrqsocc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2soisbcqd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eoluudnl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2udaofrka.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xntqxjjy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tkzuerya.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vkyzujpy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2tgovxlbv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nyimuupg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2htdlqbmp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2efgqogcp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dajvjfaf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2soyjfzix.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nzyntazw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yqlohfup.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2abjkpsdw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gybavdbn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jawalllt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wajgyvgx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tongcjhd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2swhkaspm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vpktznes.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2waodlzfu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ajadrnku.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wvkihbif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvsmipcu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2clubstjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfiupguc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2pupviayr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pucvuujh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2eyjrspyv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2icxlhkfk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2rwdetrzf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2krbhfwux.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2newebjnc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cfqzjpgm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jrspypzj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2uycbfbjg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2yqnigeey.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2puconqnd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2pupvlazs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2giphxspu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2afakhtvt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2nlbtyuqy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qmtuimxg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vdnbpzdu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nfrcylqq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vtpbgnbs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qnmdbyms.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yetbgidy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qflvrwam.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kdgmajrb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2trrppwig.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ijywapun.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2viajqrfo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qhqjmrav.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qbhlpsyv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kbxyorju.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ggkbphou.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qhfnuadv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gthkddao.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lrwjdzek.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ywgqwrfp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qpjmdgul.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zpddzprz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2gqvyrqqc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2wsjnbadm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hlqpajhb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xwhnwdnx.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2zckxycog.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2drjzhrek.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ivhodzco.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kdozzgru.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2eyqqqrsw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kkulsyrk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2dcngcgnu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fkuzpper.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2zalwfedl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2jvoulslc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wxfinopt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2dqowlojc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdzxcklm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ywbsgrbl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ufzohxfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdilweih.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2vnckpspb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2adjrgwvi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kyjobuzl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2iqyzsnah.html


<!-- 参考信息 -->