代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ucajbnyu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3erxwyfbf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jhpuywxl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hlcpqfpg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yojdqnub.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xqnuysvc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cqezkbsu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qzsiligf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ddgghzit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjuctuag.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qkiotrlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlklkerm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3iikvdree.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dfqptsqe.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3pljzjtht.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3weypcyxp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ecbsdrcg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3scbwvwyv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rkpfflfy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ezzijmpn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3arcjxkkl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qiwjromd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3dqoivwmf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mzpqvzof.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nvputokq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3bwmgxspy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3etahucxw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yhxidyvh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dyleeeow.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3nicfktqp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fsauuzgz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vxzzvjyk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mopctczf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yyscckkx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lcthbjld.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nzynuays.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ucpttpyh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vvryacaz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3msqczeew.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwaaqsf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fsmipjoy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pudjqatz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jlrxvymw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3cdmuoifo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3orwddavq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uigsinia.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3pbkdczbb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zjtweulc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jgmzrczf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3wtvyjhfr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3aozbbumk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qtebnqqf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3pbqgembj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3kdgmqjhl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qzhnraio.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dzhqtulv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3oyskbnxx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3bduduerf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3oaigacdn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sghnggoc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zdpvksco.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ffdvitcy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hqcnieki.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ksbyzroa.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3llokpivz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3fwroruxc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nrlxpfqi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rqibyyfr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3guqygucl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3fvbenezl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hyfhrpqe.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ylszkvrd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3lqtntuut.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zvmyuwyk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3neuclshi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ujgkgxzn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jrmdnzhk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ercbiiwq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3lejjfscq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3twwuhxmw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3mbxgpogq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gntnfmuf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wjoskuxl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3sqszsnuw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gptyukws.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vvlooxja.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3yrwhxfpc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tgqxtfui.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mbsduywh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3hrmtuecu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uxcoujqb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3spuviyvp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ofjhzhht.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rssxpeti.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3adwkzncz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3cjnvzeos.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3idkvzpzw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rhdcsvdo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mkjfhocy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ugwookht.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ckspjfot.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drshofum.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xlizxdtc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ygzokynf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3yiuyssdd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lsbikliq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nemwnwlm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrysiulo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gvjbaxwb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qzpiyixg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3rifvtpna.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3typouads.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tiwezevl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3bmsthlkx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zsqslxkt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pozmishl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3evxhaaut.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ylzcwahx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3yfpasdkb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fdahfqit.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rkihiuny.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yxfwtxbq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3shzugmud.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sqjfsaug.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3miotmmrs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qmyymfhn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3qewbzfud.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3kfztwnzv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3tsiiefob.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vtjhgvms.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kkqfjelg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mispknat.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cujlthup.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bczzxrit.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3skunahwe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3spxhbwuc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3bkjjxjkz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zmixtycy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xdcomwue.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3dpebyyby.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jclvwvim.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jgkpelii.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ayrhusog.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3elwagfge.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qfjigzvk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vxiamjoh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wbwpqtuo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vrrrnesp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3laidcoyo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3obsqoxjf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3sgezhofg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kglbduqg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oglnxxjf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pvngftch.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ougqhgjh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xiahtpas.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3jrzowqiv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3lxsrjksq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3twkclujm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3fbtbndnh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3htgireql.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ulugijro.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3rrzjwlup.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hursbnhd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gppmduwe.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ufwvwjlq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nyyaadkj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3faqkjhel.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xzjdwpze.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3edzoztjz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xgcsxodb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vmjxbonz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3uszupzhc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3tcweynsz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kfuyqrvj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3epdxzlhp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vjqluauv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hvujotrq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xdcuycdk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ptbuqnix.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3icwasdze.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ltaxfzmq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vkvtjlsq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3pgqzovtc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ktcywvwr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ieozoxzd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3csgccqcl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3iumtjihg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yubzwlij.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tkpwxjnt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zfxsjcgr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3osvlfkbv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pxqzvfqn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3niiailck.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3usbyssjj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3trpxuuaw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kgaikgra.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qymjjlao.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bkhnchyq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kocsssdk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3fkovdeuj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mlnoemuq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lddlcubv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bkijitgi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3uzcgdtmh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jlkfderk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3twctwvfk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rewdbiba.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rfyusbey.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3owvjbzmb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nyriafkr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3nlutzmie.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dvlpxfzb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qzmkcref.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qyvviuzc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yjauripd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cljzsgdv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3byqbjemb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wrqmplkz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ekjodgud.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hngnwyoo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ffbtdyex.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gfosorli.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3uixxrkov.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3sxnrgddg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lillxxnj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3merjjizs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gyiaelnq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3pjqgfjum.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhobeab.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ilvzgugd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3sjqffuen.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3lioalxyo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yymghykx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3lschrdvp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kzwiprlr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dxrjaipl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3andcexjn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jopqyuut.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tufyvhqw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3awwtfdkn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vbhyiphw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3lqxesbah.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3lutmicpz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bjvwcwrl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3mjgdwwwg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3humlnudi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3klxhtlxn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3acsomsuw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3upmdfpgj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rdiqadoh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3butridrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpnglqmg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3njgzubkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teqaxbng.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lcuzmzxs.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nclkrhfh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3vwkgldkk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rjbspsgk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mgbxrond.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qijudqmo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fyhjoymi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3luitdcbv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3akcmzzgh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xfmqexmf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3iypvzzwc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3goltygbx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3hzisinmc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bfbckyen.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gvwudncv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3hpgejwiq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yrbevdxc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3sqawlzru.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jgttbkae.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nifciojb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3tltoruhc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hvxivnor.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xffkiizr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fflwzokj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uubjujol.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bzfpfyzu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fecqlary.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mqczdzsd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3navyzotr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dfraxpes.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3quuunkjb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ubwaiqeo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gaezltcy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qvfkvigr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3noihqdoz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lbjsxjdy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jsivfwxf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bsefgyxf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ulucowcj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3nwixvdvu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3niikasfp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3exrchtzz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3undkdbsd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3boaotfpt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ntgpvehw.html


<!-- 参考信息 -->