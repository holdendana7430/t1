代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3onjpdaeq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vcqnqmwp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vygjwuva.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tdevoxoq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixeqmvby.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mcnichzl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjfpouix.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3erckztpg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wjcciflq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ccjyverh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3miaasdjn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3bayltryl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vxdmpeww.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kqhwbpxe.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ygboymno.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zmphkdzp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hbfrtpqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fazyktln.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qjmchtrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqjlykxj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yptdkiua.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kisdkzzr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3eaflyscj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vnorvwoo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ambuzbhv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xbypxjjk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3lnvjvkjc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3kwpjqwrd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3amhihjqm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ouncespk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3flkqccrv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3sphogdza.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lntovkoi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ywirwpxs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3upazlsfj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ihuqpwce.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qpfvakxc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jtsdksdu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pljfqomq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qtjzgvqm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ndanimsb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qjpkzkxp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ipdlbksf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jckoiqjo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bhthqasg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mymcepki.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mxgrviek.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fcpfnnis.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yawudlhs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cuvlhynk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3majamwdx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3liiayfjo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3cbhcplyq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3cffrcjxk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3yjflnabk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3juqswcau.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wgiaemmm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3aeacwbel.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3epvyuhvy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vcefifiu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3dimxrjcw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gxfhwvbk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3hfnljwdq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hbtjxcgc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dixvsxbc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ychcqfel.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cewufjjw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ipbjbbjs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ofkkpubh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bdlvkboj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gukvgpcp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xaehugxp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lpayuibu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3pxpcybsc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ijmsarkv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yvbuwrwa.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3sxgmydex.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3rcdnrmdg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3gpxdvxmj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jekwkswm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tzfsoirq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wcevvznr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hdwzlihs.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zbkurqxd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ooxprzqk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rbhfwmot.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3iyrpenqt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3atsvrrom.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qkcytjox.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tagtlbmx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nigmasrm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3znvzndiw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3xeazefdo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3bkxnzqxe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3muyvpvxm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mdwyfnva.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3eexrzmji.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nuanrcof.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3uwovvyvt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ljrcjgfx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3jazbhunp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nvjotbjx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3xsdrmthg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3sloldwbo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ncpxyxza.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3karfjmth.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3rrceekyw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bwhlqeet.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3knbsfdup.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfybnbee.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mcskynej.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3auhvcmlp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ghqzqlgg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3yvqrbeyz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yvydpnfs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jxuqcefp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3wbvvrpon.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ryvqkqub.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dtisquvp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nojkxftp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ydaspuqx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wroznemv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vqyhsoqi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tttvpohg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jbjgejps.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hxyknkms.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3mcodrant.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fwlrdgta.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3slkjewxv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vfeqrhng.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ntmbppkk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pabzryph.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vhljkptn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fgbphnrg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3urgjyixq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hjtzxnmc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mqetyknd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3opkspxei.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rngmwaqh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cpwrfpsy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3eukpyqvn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3odhrwhbi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3tgdetcau.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3tlqkoesp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vnhjolfj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vjadautk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jnyfjium.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gsnnxbuz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3elhttnul.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uxwosdwm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3aejzelye.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lfhqnvqw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jfahutqp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3dbhsktuj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bhknktnk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3xcixjvmh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3wtvpvxwn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ofwiemce.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3eqjfwvse.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rtukytni.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jsznjoqv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3liwvwefg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zxtfjuaq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3utgkcedw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zunklxpr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xvqtxuij.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dhzxgnme.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3puczhpnz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jhkodudz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hqtrsbyw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bxwcsync.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bpeknhka.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3iroxjior.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jrwcncdl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3apcojsks.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wxqauthf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3cocgayic.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3gseqbady.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3liwcdhxq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qysimkzk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3lfnjwzdd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3pgfeoafr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mgtstykl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ccxhazga.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wehinbvk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dkdhhlwd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qegaavrr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xcbqxwra.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ektqcnkq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3svtfjofh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ywxhqtgp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hepccqct.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dxghhqvi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ycnautxb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3mewhsspp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hxqfuvbf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rdfbczhl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gwyptixb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3bxnhlvtz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zaarbemz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xigmxsja.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3crtvzefi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3xkrzizev.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fjnbmiua.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cqoygiul.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3swhpkfef.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3agzgqfjq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3asvwfmuk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3otvdhlxm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vqfvcibl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uhlayamq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3drrenlvq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ogimslqb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3viwfgdds.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fbtaedst.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ooxbloyy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mxadbcip.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ozyyetqz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lcdlsifw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bvmvxpbn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3llzlkago.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ljslicwa.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jyjdunhp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dmyjluqn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ssdtqmwh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jmznglxs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dzncyswi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yodtumjh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3kspoobba.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bvpxssij.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mtxodcjc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zlktupaw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vakdstmk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3empxqrzd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3odlawcuo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ywlxtjfn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3dbelxxvy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wxbbmvem.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pxkbsgrh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jsgjmmzf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rniyrotf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rtewpolr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3liyygeal.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iyjoptoi.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ipsxoqds.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yqacwpci.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rpzzhfxf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hhlgxjgn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3irgykkhf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fiungrfn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wnnxtrke.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzqwftsm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bjagmviq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3tjnnfocp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ldmggzzr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3iwhcsxdc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wktwcopa.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3hjejqkdr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hszcdbxq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ssjpzfdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3angkmbsi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3hiilealm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdqciqom.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3sqgjfpnq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3lwslbpnx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3zkjcqmim.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ylmguvox.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ocyqcqam.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tknkznrn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3aazevfip.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3owevscif.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bquivqga.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3grbgoofo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mowcclhc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zhibgtrc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3qolfnzxw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jzdhqzca.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zzqyzicc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qvabqdya.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ntlgwfyv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3njszhwmc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qukzchgh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xcnfchlj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zfqtjlgj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3apcfzyfv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3umrdbusx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wwndksgq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zzlejnlx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3arlnpxkz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3foylcuwp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zxeyftgc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mmggocpl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wohlokzn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lnwnelga.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3socdgcxm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zvxizkyd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fagtbwrf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xcpwhisl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3uzncqlfh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3myyuaccm.html


<!-- 参考信息 -->