代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aljgnaqf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dlzcsjaa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwwzmqcp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xlecpeex.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tmkputgz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sdbejtze.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3osbgiqae.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3rayoteqy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bfihtjlt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fochxqpf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jvabymwy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3atmjqjma.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hljxazut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjixykfq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cwlmiyer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gadvjlao.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zqzsioef.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ipschauo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rtwacjen.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wenhhtiy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3immbjeaf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ghfnnscp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zdfqujjp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fwmiqten.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3anqumwtz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tqfdguip.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ajvqkelu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jkcqudwh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fuunqllk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zltwjobt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tddfyxdv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mhjjbocr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xiaadbav.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3pxqptoxo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dnuefkrk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tppaoyfv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dsqnyfeu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lawsvoio.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zdfhuuhw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3okpnthqx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3bxqnzeoo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gndclqem.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xpgqvbxb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kmfdrexf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rbdmdbxa.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3yhtcddmr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3wuejanqu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lftvcika.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nqzwauvf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jcewrmvf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gutqooco.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hmkzzokn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wdbybbls.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rhsqgrmf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zcxsmkyl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ttgnwhke.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nkzwtfad.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3njefrseh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3shssvlon.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rnimjoap.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wgpnulik.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qaigrtug.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3icrrjepc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vjgwazkf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3pkkysgoj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hjohvylm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rkugnqcg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3oxzhazwo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zeuwcbzg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rtrtwjqm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qxldznfr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3sxwqileo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xpgfpchr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rsukarsb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zhuekqiz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqteehy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cjbwbkmn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3yiketucv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3drnsisru.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qskkxhuy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3vijdqazf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zjtsvtph.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jbzcbkqt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cpcnwslj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qmjqqnps.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3dpmohbvw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hahsxhui.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kgrmsivw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tbyehkvk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hgeaaedl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bjyerbwy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3geaszwph.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jcufpufw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bxmqnbzi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cdiiibhp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3epzwtkir.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gcndxxxw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xseirpnk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jkaabmca.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3yektqqbk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3apaxewhx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pwhxpkky.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgptukdu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3favnjxnd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bbmvnzmt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3acszqldu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3uwldgrfy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dbqwedgi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hcusuagu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ucjismdn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3woqgqamy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3otveryrd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3qdgaesiq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3lbjokuwr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lcfofope.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mmkfxoqy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3durdtfsb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3sjgrwutr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqyhiydt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xawsgghn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vygbojaj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xcxkzaai.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mstlowqq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3rysyarvi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gkmcayjv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gbdwbaxq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3acqeeoyg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bjxjyuao.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ixpxedtg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hdtpksrb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3soxyqhgj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ezrhjhkq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mbafxrem.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jfzqppif.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3awixvkyf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fcsnvcmy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3rrlkrojb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cbmvwooi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ecrmoioq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3dpdlhqth.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jxeyhzho.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jpdbkvkx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3bnikzrrh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vmkcbnnt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3tjaymdvr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3deqlzmqj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3zbaqintx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rhgfrqnc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zxwapsip.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fjwofwub.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yqkqwyzq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ktnncwpt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zindnhep.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3qhdoolqm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3sirrayzh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3yzexfnzq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hlcobbls.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rpqrvwgl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3awvwzpus.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rbosihla.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ltqddlpk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3saxxfeyt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kgqrzbgv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3acbwgobl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3glnbmxjb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3pnljxxik.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xuldbgdh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3embuqeoi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3uckyqmtv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gobxrqis.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rhorxaec.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tebhmiep.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3uwvacurk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3rvznjlvh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3rshsdbky.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3nzgyyzrg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3zfrewjtj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uwvhrvwp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ugksjmed.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3czovdtux.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3bedozlku.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3czdchwkk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xodkpwbp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3cjlqlljt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qritebyz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tzarccdk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3penoawao.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3yxmlyzdl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3syzjtnkb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3axlbdgbb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nvjryidt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3slvaydhx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3udcamjkv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bbkaxllu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mrxkyeiq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qgsnxxst.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fshziqzo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xmwugtef.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wpavaphx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zzoryvqd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3djgrgclz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3symghoej.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhqqcwno.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uroygivy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tpymlpqt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vvvyocor.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ywzcjpyv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3igjttvbe.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3zldynpku.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zgkzraxi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eumylnku.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vgoltcik.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3vthromjm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lfjrffrd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cocnwguf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3gmcehnll.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ygorzcql.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3yklxfigj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pxymwdkq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3boahfnjq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3iygytoeq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3poalceyh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3uagrcpsp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iwyfzkho.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qgpujvhk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3javrzdnp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mrpqmjqp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3cchfrxnw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rlgaqihd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ggnctbbv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gbdiksxl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3etehwwio.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hmsbrjae.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rnhhguwi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3dkjizjgq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3coulvtpb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ncxgicqb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3xjtfjlok.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xbwjslaz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vdofgitl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3johhfwww.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oisixodi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tpxuptmd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vylfxcle.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cczcktvd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zsjuaqnk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tdakrudi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhbbcmcx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zhshbabx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3etspdvec.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ljdheckl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3urqbixwb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kusztaoy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3uzwgybrk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3lmiwrzbw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3mlhoppmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3coqbusmj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3sqdkjazm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnfniljc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qcxvnvlx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3iaiqprhb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3emfnwpdg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rplmbrpb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qlrhleve.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mjlujjsi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yrnxbedm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mhdawrge.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tgfwvfcn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nngwzcyk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lnrytxhr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3uktduzyl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3svcdoawz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wcfrleqr.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3cgtiqmkz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3hkshcupa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3lsyvnbhl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xooglqcx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ovrxxaci.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xysuzvro.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ekehlljm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lfwmqldd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ddjujmcm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3arhdpkob.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3onczdtuc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3aiuygqoa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3uchcpjcr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3grdgkwpn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dxwllsms.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3szoncyzk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lhoukojk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lpcknqcx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3evbyvvfm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yqkopdjq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nljdugth.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3osxtvfvw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ghdybpyq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3svwznbcv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3jxfhtapt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3uwlunoyl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lmdauijh.html


<!-- 参考信息 -->