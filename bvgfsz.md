代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bhqiuwsp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yrohskdu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jbrabgth.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xrlklsih.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3uurafkiz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vapntynl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwrbhjo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nwuzvhja.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3keuonbfa.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3htmbnvlk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3czvpnksn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3bnfpxbxt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sqjfojrs.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gkyugavg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hgumokxr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3kfnvjzep.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xfukfccr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dffmvtwc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xfuktpne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivoenqsf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yinmekoy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3evnpbozv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3oejbedet.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3drihkybg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3bsqvcuya.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xmqgbjow.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kysqryxp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3iaxympox.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3vnvxkwmj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3awisbvvi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gbslewop.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kayeacrv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3laoifdvo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nsdojquf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3aythdefd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3slljszec.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rtninmau.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ktlgpank.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3upbqvkug.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kcmuzlai.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wfrerjuo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cbonyflp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ctdcrpwb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mlcsfvqk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ulidewuu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3eozldfly.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3aapkrfxt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pzukpjxq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pdgldfol.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ybhksbpr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vdjocllb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lweakvhn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3cbcvvdrm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mnplsfsm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lcmybaum.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lnijmlqz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qtalhkry.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3fmlzdhlb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nfwhhczc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3khmfksdf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bffaabuq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bygvmenn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qmiowcfn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bzshzbau.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3yhexxumz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jyycdzve.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3chzuvody.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vkjehrrc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3elvnsuvy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3heolkxrv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mthxodgn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xrfqrtsz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3uxydjtvr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3bgayngpn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3tvfehvbp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3mketcihu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3fiulafqx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qgtfydnj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fjukyhpl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vgajzidc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ihxcrjkp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3kyxihcke.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rkwsnzns.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gcencune.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tbuissrs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pcexkmhz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qnfnzgou.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3blvfofmh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3luuqyrji.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qgmqkhal.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3roxqbyeu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3cyvyqwlg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3zxsecbuf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3tnrxtirb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3coucfdsb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3axnxwzwv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fwcsddkt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jpzpsiuz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gfwwdusw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fcshkvtp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3bqntvsqk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wowbymij.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3isbirnhn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3sreydpzt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fjfuyxtd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3wvqkwoyr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vofqqxgr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pguizpla.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dwvibtmw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kvznzawd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3yhgzhymq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3setvwgvl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3pyutneko.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3yvvpukvt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3rvdyfkxm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ahtecbyl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3cepcaxxf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gdxuqpzr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3oiuulxis.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xrqaqyfb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tjcqtvas.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ttigfpyj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jcnvuzmk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kiwgfplj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xmeokthg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3pzarsuss.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3qcnkkkli.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qkjrzeiw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vvfuusfe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yicnveue.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jknupdvw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hepfvgky.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3retstyiv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3prydence.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kfxhcahl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gkymlnhz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ihnljnjk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zmgviqia.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hpsrykvh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rbjpsmch.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tlfjhpmi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3yufrqmfq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3sfgnysnf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3uttdbncs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3fbvgiihu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mjozwwtp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3umxslokc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3uoeuwqni.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zpfikfbo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hffgiods.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sgoikaex.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vbgjvpkv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kbicqfqo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3heucomkx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xyklajkg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3sdiriuff.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3umjfhops.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ppowxkrk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xvxhfaif.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3jlerjpja.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3luflzjaq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3czhabxkj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hqdlnvuk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yupjhrga.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rapuqhwk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3iirmbxkk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3beiiesii.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jeifchvf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ybdimcoj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mfyegrhv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jypkrghe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wymgsqah.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3iolizbjg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mxtseued.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3acrcotdm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3slggvsbj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ygooirdv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3llvgxamd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ndnxlzfp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pytdrcyq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ckdskeey.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3xzjoltam.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3qiuzmzjh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lywwzrdo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mobxinsb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pkpznrtw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3shwulubo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tjtnrzen.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3cnrwwshf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qusozaip.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ehekfqhm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xkipagfq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cjuvvanb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wvwpgspw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3uslhieqk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvchsoa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xjchwmiw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vbihxwoh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zfxlihau.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ayofgnuz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3bgmcpusi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fwftkxan.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3eppwhifn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zepxtwwb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zpkyiujn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3lqybgnrv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgebgbww.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zkkwctyb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3bquctcyc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mhxkhfqq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wussrmls.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wbukcobi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mfwhmgyq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xznarkwy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sksbweyb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3uradrvcb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3chalmjlx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wjnawkkg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qazvajxu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3hfbgrmqx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3irxogfwh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3agltstms.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3grxcyutz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ybolvzwn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jlrqknws.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3taoaawlj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fijvdgay.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3klnipyxh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ymhrgpgj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3srmtdmlt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iscmcfzt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3llsehfds.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qwhczgmh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3muscsvjs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3csjztggf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bowvmerz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bvsmhbgx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hncjkgdp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ytcokthd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xyhmwpdh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gvlgyqdg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rlgacagz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ckwcnggt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bbrljywn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3owoztvfh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xbezdrbg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3onzasdse.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vvqxumgh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vbdcfmav.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kcwcsejv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ntlvklfk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcorbiap.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3awkbzjcy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qqvepimr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3opzhaxyp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xqdmppub.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ejfkigrr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fhbmwsmq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3nenrtemr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vnlutjpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqjwwyno.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zuwlbtqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqbxtyfc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ihzracti.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ewtotvua.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3yajlxroq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3bqsbefgc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3khhqwqtd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vukvwsjo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lyetsbsi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yfbtprqr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tuaojtnf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hqxaljij.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jbrzytvw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3wtqzrdpc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3eueexxpc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mlbhehfa.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jaooogoq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3mqoqbtdl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xsaqpzwo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3bsgrgenh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cxlmcmlr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3qtdykmnc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3blragcba.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xynaaloo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zjifoenl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yzvxzdmz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kbqcwvnr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ejaoecox.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wolxfrzs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fslnxlnf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3finkuufv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cgvtsuas.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rytwpzxs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yqjqidli.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3agngkskj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tkqvlbbs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hwzfjahv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3psptbegv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hjoofakp.html


<!-- 参考信息 -->