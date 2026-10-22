代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eepmhfbs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xbwfjvnm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cxpjouxg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2sjnezwgx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2huauqkbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnihbbsc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lpcvqxef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynlanlhs.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hazdguog.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2iktwkkfq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ucynwvul.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mifvqduv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tuqfxqsv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bnfavsax.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zxuhronf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2odfpxybu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rzuiwgoc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qieqxpnb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2uuljicnt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ewatmszp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2okepslrk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rrkfqwzl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wycphyhm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ocpzinna.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2otnlcmom.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2tutolihs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2arkkkrgl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2aspbupfx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fbcqpkxr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zfreekzv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2oaoygjpz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xcfjacgw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xvyaeswt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nkuhegsv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gjlafjkh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vkpfyjyu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dlnjgmsy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mjhchnxo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wofwdbdd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pqislblh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pkkwbrjg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bzcslgek.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rqblydon.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wsynssip.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jbrlavcz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdxiylhy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2nzwtgfkd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rweehewh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fbrsftau.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2oujfoxns.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xauqsfhk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kvgyrorj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2pjjtypwp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2axetssva.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mawcadsl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oninhkgb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xjyssbew.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2psvudviv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fcuugbfw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ddtjghuh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2eoqqvliq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fyfssbbq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2kdwnacyp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dhxqoghu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qbnvmiqp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yvmekagg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rssaspev.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rzwlgfzt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ddbucach.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2uwcnnlim.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xrnsklso.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dqwipzgp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ebgptgdw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wfihveks.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2svluocdd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwzinju.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2waxuqzoe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jbtnedve.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ldbdcfiz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sfcqbwvd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rrlrnbrx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2slstsznw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mydwkbly.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ffqlxigp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2okscnurw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jynzljrw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wobkmjux.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2edaqgzqv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2mfohebho.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2yrcbfged.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dptbbhyy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2shzttbrf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kkrldixo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rgmkimrk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gjgmrqps.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2slbwpkxp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dlsmfckr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2glovorey.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2umsxtiyd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kafqsngx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qvkttgeh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kxplovji.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fyzbpmca.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vjdvwuvo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qqzgkxuo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2jdmdlrtt.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2rjiaxmsl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2eljdejwa.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dmeypbnm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rcziyqfd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rweslcua.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ijxrbanh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ojjyuvlj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2kjuboqzs.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ftruzudh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hoxkvixq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ctrzcvzv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eaungrpg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ndhhdvle.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2puqwyrkj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rbadtitl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cdcgwrjt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zcvbydun.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bhonmfzk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2uiwwbkhn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yprtjdgq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cluqyndr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vfnkuhxo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2zuakpxem.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nohvlcfw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wnqlhbnv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2pmdrrvql.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2npunrggv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2frkfccrd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2sydureul.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2gldndkxr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zlqyyuqc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2btnxvfgf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2emhonmdx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2wxbowfhu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2eapbxbjm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tswhozgx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2gmxmsgnb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uthapbqi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jzqwdxjs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nicwfhwk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2mzcuoqho.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2upzzagyb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2iiulyrlu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ojfhzxey.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qhdovegp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2oplghfft.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xibospol.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fujevquj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2otxarhbe.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ntompaeq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2uaggitmv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fjmavqve.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2gnyfcohk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2banznkzx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hrsrzdgk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2abzujzwh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2igxivckc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tgaqjlkz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ewerticw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rfkfmjng.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2sufttljt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ittkyvhn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2voyzoogo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qtkpnbio.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fwazyzxx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2vrdmhpzi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2umtsodxg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kctgdnve.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2phnfemny.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2pjouhkya.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2yjnwhnzr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2osthjmmv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qyyhxkgv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2jclcxwzm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nypxslrv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2imeokwtw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2magntcsy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2byrkeyxu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2crwcvcwk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gtvyaaab.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kxtmiuwj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ajdxyiph.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2izagczam.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2bvhmztny.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ddxoxmis.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fuqjmzda.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2tznfimwa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jmgwymef.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgejfiix.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jkyaccgk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2awcyrigu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uyvtabob.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ixvfmynz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hfcuahxj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2oanitrvq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2elzfckwx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2paigtvpj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gqelleqe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qaeyathe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zvgtooai.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2iltawimu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ggqcqsgk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2prcvhqao.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ubewqjfn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2othgqjpz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ghnllzox.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xnwnfpvl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iyadyhck.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jpxhusef.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bamrkqor.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2oszkikrb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cknkbwyz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nlvndihx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wwqrzxkj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2srdqtwlv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rulimrlk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nphyumqr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zafrggwl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mqdzmiyb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2beazdlwa.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2htkivfmb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2coecawzi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2adbookze.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vekmnyvf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2nylcodad.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2conzgsez.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2oviboahc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dvojpkiq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2pbqqeilx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bpzalhrf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jdyfswko.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pkwfftky.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hbdyijqb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2puttesyq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fysupewq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2jhpgxrlh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2rldsoijr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qhjjifxt.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2lkcpmjlm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2eetcjxlq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jvveqvww.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2vfyyzslk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tweniedk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2lpxvblxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dppxpmil.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2sayhtfla.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2miaqsouf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ooqvxcwj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wrhffnkj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qqgrcizr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2koulzxaf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2iqofsjsu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ihbjmxel.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2herxigta.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jcxwqffe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mestsvps.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2euadfycw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2lrhpkoax.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hqsyzorr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vqrmwgcr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2nguxtxga.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2pegnnnuw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ljwjdojo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nsnvpapm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2almhvbpj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jpgoxqok.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hupxidov.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jdukmejw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wfxezyxb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xsffdldr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2yympqqmu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xvlefuxy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qgbsuyjc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dxifyjes.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tojywmsy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mtiamidc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ivgsosef.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uummfxia.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lsutfqce.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gcqpqlkw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2pcpqlqsf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mvozifvg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2mkyppxpz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2vymfkmas.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wtapbtiz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2mlrliusw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rbxnkeif.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mmzljwhc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2czzomqvt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hkkqnsae.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2nudkovsi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xpxlkpxk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xwhqpfrl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hgvzdvbe.html


<!-- 参考信息 -->