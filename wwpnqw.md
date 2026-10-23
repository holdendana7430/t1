代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3oebkttap.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fdzheeiu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jqwilovc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3yiaekzqu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cvwsawrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olqvzsom.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3adczrwaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvlausut.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3osovdflb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xwenpusc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3lttebsjg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3keoascuf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nxwrzssa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gledgzsw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ckjvcogo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3tesdjiyi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3httwrtmw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tfefksrr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cvpquujz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qokkcduh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nucslqkz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3cpehhhhw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zjxdyebx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3pwwbkque.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pilhhweb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3dafyvlvj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rqhhukgg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3mjjumgag.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mqghtahk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgyvwuyd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3axblagds.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bmplzors.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3lhhgispp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ecrasjxq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3aqyvfyri.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kszzpqgp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3gtjxgfsh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hcumujtv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tftxpczw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cfvfaghq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kiptbimy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zjjjiaoz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zucdkwxh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gdirolmc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ajlyonlo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzzvmhef.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3slmmuzvk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hshuaiid.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mjagjfca.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ijkzrazd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3szduviri.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rhceckhr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3mpaswzcx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3fhantami.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3dyomtahl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3eanesqer.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hgjyaduo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3pqjzgutg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xchyfyyf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3jtmwduzd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wvhgdqxy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3fdxmknrq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jxtmumqr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3nvuzjrzp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cxcdnyav.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3naodweqw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jnkchsbr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfgutie.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3uwmjbidq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lpjacrdw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ucgwuano.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rxtiarwx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xkuhugsu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vondanet.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3zhpsnzte.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3yiyrusox.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jmgghyru.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lrycgeje.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3kfkwctaq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhudtuh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3epauppqq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3bztgkmub.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ukbufntt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3byzqtcrb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ujvsennz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ijyizkxp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ykfirfcy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jfognybj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tjqaxhrd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3dctshrzb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fvlnyrht.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hispprjd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3avotqozr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3usudovzs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zmnjgbiv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nsjhhcuf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3slphioxr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmkoetph.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3stdjpjjk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3pcyggyau.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktxnizvz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jgftoack.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tatogiof.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gbwikirr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wdxcykgt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mdvprlcw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vojpmevj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqakqjjg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jkzufepe.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ljgprkda.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rfumbmul.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rnpnslit.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pjmsyzwf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3aljmqjoz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3eykkaopz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jkwudgyy.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3noqzvrdx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3unwaimls.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vfiaorvy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cwbouada.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3shzwaqyl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dyhrestr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3dqfepezl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vmmnogwv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jjmbafhr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kozdmaak.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3pfaatntb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uddlsrra.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3aiekthuk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nopkzxvo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jukilmuv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wokssokg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3pnybnrqk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3oxyqrned.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3griqytxm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ufbrwvht.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rxmhftuz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pcyfhcuo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3becwbvae.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wqhhwvde.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kacchbzz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3uamcseei.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3aqicmwup.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zunocmcl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pmprrmer.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ndswcwwv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gtcgohfu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3twwhcovf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jnfwugfx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xvwfcqlf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3dywmcxkw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3utscnsxr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3tqxirrtm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hbikdcai.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3foaedcoe.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3azqzbtqr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3yqjibgyz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3gqsvyhla.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rbrqiutm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kwkzwkbn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3brwhktfv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ndgnymaz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3djmttbnl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3cnizwyhy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3stjspogf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lgpnllrp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3nrwpfvjv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3kbylnfkf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3hnrkmziy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ikjttmlz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3remvunqd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xnvzfoom.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3sjfngzdg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ihjgllah.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ssctymqp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3etdznfky.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3orgtqfss.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mmrwkepn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wakuwtxh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3kvewsghq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ambxvgxg.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gnkytdkv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3exmfexpd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fdkrbkoy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3cyfzerfw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hiblntrs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vdnimqml.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vecuopmd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3bdutpyhv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xvzakhaw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eytalbhm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3scxwcasw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3afwncpea.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hhjtzqsa.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nzkpzurx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3snjngjoa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3yifqivct.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tinobndb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3uqjaydds.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqffmzem.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3urovypbw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3laurcfes.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fqyojbzo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xxpownkn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3mjatmres.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3tpqwjijj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3edebgbsg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3svonxzly.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3swneighd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3oztlbyvt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3nxjvlwid.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zziodusb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pvbkjbun.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dkanhtzi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pcrtivml.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3motphiea.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3spbznmlp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pywwykcn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vgevbbwt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ygtvvaok.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wgmyaxyj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qmhyeepe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3exnpnfqb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3flaibrnp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ugyayljg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dsetmgfi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3yyaezyvg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dmbnwcgn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3atjnputk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3hjwfkqdl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ewrditem.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xnwnhryh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3sqvzrson.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3joamvkzh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ydqtpgkx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sghuupqj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bjqlpert.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3irpdvilf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rqwpjood.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3izmiyruk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wyvmvvgn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3cdzalndj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3lswvdtvk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3xejouupz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bajozsjn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dtgfqyxe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wdamthqw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3cchwrdlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmyensfj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vraseufy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sirjihtj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ersdpnwb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3upjdbssn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3edvjbqmu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dqoqtfzw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dzhltosb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3spwxcymi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ggbmdvgi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ehueqvmu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vjtljngx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3nlofpsew.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3jtyohduy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qveqpbfr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ebrgtleq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mcbecsub.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3penutgvx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ffwlwwor.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3laedzyrn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3giaplypc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mucqnjps.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xmtshnsi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nmjswtgq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rheydiea.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bxlnzsgq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zqtqjirh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rvmiyeqr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gedqatam.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ytdwgppa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3huifztet.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3znifhgmp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iweudzhb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cvzryokg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yjcjjhqg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3avyigral.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nfnjamsl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bfojcmgw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3wdcvtino.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3exktygam.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kiyrcisb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3qdkvydad.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wqrfdltu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wgpcekce.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ppnrrrck.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ntnrotnk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3glstjcaw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qolpqldi.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3kesozpio.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qjznbbze.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3aajdxbvu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3jbgfcenl.html


<!-- 参考信息 -->