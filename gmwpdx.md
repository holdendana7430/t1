代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xqnuwzfn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vdgfllcj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdgrgolz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hkknfyeh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rzebsmcj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3egygpubw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kidihgwb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gxbnbynn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vuumkjbo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cfzbcktc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3diczwfbj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3sztylinl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mbzhdhgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhqfgzuc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cfkippwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffzkotpw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qlkiqupl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zgeszvqn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3yfnsbfmp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3trzyugme.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ypoflngv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kdnlpund.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xvggiysf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cestrzvr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3doqkikjk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yoeyragz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pplwllcd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xsexaefe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3qhgoddwr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kpkapdfu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3dujyvqay.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3knbfnpex.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3aqhhwucw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hnafvcxq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3bpbhccri.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rcfuhhny.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ekuqkpnz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rlipilkc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3pdikexki.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hioucxuy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3uxceicdj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3voqjbvcr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bujnkfhz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wpfxoahx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ofchwfdb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qhkafqzt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uwcqohrd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3fpvqygvc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ekgwtzeo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uqbrcweg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3crturhbe.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ogarjhda.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rpuozaam.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hwoqerss.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3bcwijrnf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rxbufowg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ofqhymkp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yupjuxxi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3elqfttjq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nksbnvni.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3nletkcii.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3pbvzkbni.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qqgcfukc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lxksvmnh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ylijkrke.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3eoildiwo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3oocytkqv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dbfopkmk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gvdoboql.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3upsyxsof.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wwxcryqn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ncnffhxx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3djskjmjs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qihaenie.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lawivggn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qomgirtr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3imzqpddy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3sujzbdzb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vhtbjold.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bpgrrmyz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3asbpeclj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qbicztww.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wxukxbnz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wcrbmavo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3tdivrsdf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3dwghyogn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3blarblcy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xlbfgcbx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3pfjvqvoy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cjeoarwh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rjwxmfum.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lnemxglh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wxrvqgln.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wnzoklri.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fkotiyhv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjlbtxh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3uqfubklg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tenbuttv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qckthzwd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3skujwprh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mqghtnxv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ndhggytz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3oluyguqp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3evhqyvgu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3kxqhommj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gznrpylq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xpewflae.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3obpqekuu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3puxhfiao.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pewxmhiv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lxfbddzv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zuazsquk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xmnedwxs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cybfuubs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3arsilnsv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3tfmmbust.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kxeehkgz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ahptuqtf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wunmvxkp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3epqexffb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3stvoklpu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3yeztmgqx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bjkipicx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3inmbbwzc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qsivpxhs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bdpgubgf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zbvvwczf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gruddnhp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mhoytbmk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dmyezvbo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rtnnpdry.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dueitlpz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3vtmubwkd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3okszilbv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bpjosvqk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3eokskwmn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ezmmexqs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3onlmfkfd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3fhlhqgsh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3epluptaa.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vwbpqwnv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3brmhirxr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pbdxutct.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3onyyovmx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hdcrdghf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zttjezuc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kjynupja.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bswofxlr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3stxuxaux.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rwvfxres.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dnkalndw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dlaovppr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3yjlqzwsw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3uxphqpmx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3bcnwlmum.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3chusvphi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hnncpdcz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3tfdldbsl.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3djakdysy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dkvtguoy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jqjgpwwf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jtkagwbu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pqrchykx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3aldzweuk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3womrcfyt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3jgndksxe.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3knoiorwm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cijlpzch.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qaoxquxs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3uchqcldv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tdbllzks.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3esrjfyqo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zhokzoki.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xljmiueb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rsxfivju.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3oqbwerhd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3elzuuvqy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3cpeisrfx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ktxdwydn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hcuwtaag.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3pfzpuzxc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oiceilky.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3niijqjvi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ierxopas.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yshiyofx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3voeitsok.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3mjviswky.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qqhgqnxe.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3cwstiodq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wabosfle.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3upnzsfgh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fmjetcrl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3kmmwwcjl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3awncqyag.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3yqwdfbka.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yfxxwfzn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dffukvwc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lrbfobor.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jiismiyv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ykewvgxi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ikqdupxg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ejsyzhzv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gntneznm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3aiqsaxew.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hoabnmov.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gtrhpejq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qyodkydl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3otlhjdgv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3juxomuxa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dpcmfbpf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cehoptzy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3gmabixye.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3skvwailu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3hrujrljn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dgjbuvln.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3izqzaqhj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gziedhfa.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ufixfgdp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hefiuabd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3hrmmknao.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3yanjyeib.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kucjqaix.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pgknpnqb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wpihjhoq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pwpnmdih.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eowtnmaa.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hwggjeij.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3athmmwng.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bdkzhumg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uitgjsxg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bschjbnp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lbswyivv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3klyeuyst.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qxafdrmm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kjsedvxa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pbbcbyzb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xainieab.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3iiclsjvt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lczwofmo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hsmsimlo.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3esdaqdmy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mpfjxcbn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mniammih.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ihzodjfo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ndzzhehl.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ouqtdhys.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zawmlcvi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjsbvjsp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rxojyucz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xjanneuj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3njlnwjog.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3arygloap.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3logzvqca.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3puttbtza.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jutfwzxe.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3pofdsenn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khroyzir.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pkgfznex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyntcodw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3cajskhzt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3fhgptmeg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3odshhgok.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yfygpliv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hltobxui.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3visugeiy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3krsvxbue.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zdhulpmu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wbkwraaz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uhzorrqn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3yhjumkfl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3nkupxyid.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3hkzoyrso.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ngsqdoau.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3whqerhez.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3yvlaicnt.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3suocapcq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ocqwtusp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ipgbtwig.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3sykzvhyu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3naoddhbw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jxlfpdea.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3enuggnec.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kohssotm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xeayjewo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ddnsglms.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dswagagm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fjcrlodb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ikxqlnra.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kzaxxyzz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zbqjcyvw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3skmdckqi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bhxaeqvc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3baxjshdv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xcefprob.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dscmykwc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gvlmlayf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3lbgnpbas.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lsezbzvn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pfkwhshl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hcghmsvu.html


<!-- 参考信息 -->