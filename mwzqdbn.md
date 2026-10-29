代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gqzwgcovq.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gtpjracmu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gnwcpvqhw.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gkartvqno.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gvvvhktdl.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/garcbbynx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/grxlllipf.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/grvqluaol.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gxtskllmk.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gdcfexrcb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gmsntffgd.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gibpwaums.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gpswojqgd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gabjjkbts.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gyzqsbuby.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gepivttpa.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/glmqxqfng.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gsfzgxrmj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gfnnnqldq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gtsyrrzmo.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gapzxqahi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gfmixxtyp.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/grptytuda.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gsinabbcv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gbzbzxart.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/geyoqqsle.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/grjuxalsg.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gqszxigrf.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gajnqiwsr.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/grrybdyld.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gzkvxgclk.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gfpcvuoqo.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gazcrnxld.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gmajqrsbt.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gsnllgjhc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gvebkohrq.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gczccslgd.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gxygmfawr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gjxmefcqu.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gpzjjzvrs.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gtsrxhvck.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gbezuhvtc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gnutvdape.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gtctrobyv.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gjevkouxl.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gubsrtahg.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/ghgvzywlw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmwfana.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gohrrdzwq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gyqzmwisi.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gwunrcrvn.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gfkjamuum.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gifxqnpyu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gixqmiygn.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/glfmhyktc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gvqfehruc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gycgpfrfp.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gzgadpdza.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gblqkbajh.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gblcsefxh.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gksegrngw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gigobjjri.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gpdpnomwj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ggfwpvgvt.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gcbneszjx.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gxotybily.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gatsyihtn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gyylpmrei.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/glnpbfocv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gtgapoqqh.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gyjhsjqle.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gzpjstdxn.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/grhiladxv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gjhtqzabq.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gwzsagrml.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gdsyleizf.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gzxfukhtq.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gevrsgkwo.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gwhdwgxvp.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gfgzoztid.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gpkxwafuc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gnloewsuj.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gsejemjpm.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gzxfahnkz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gnbhmkcmh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gavlimkjc.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gqbpofofo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/guzlkmdwb.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/guyjxixle.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gjtjtpmwe.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gshspcuqj.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gmuekbxqn.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/ghhftqjia.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gnbkzhywq.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/ganbgarpr.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/giweqwfum.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gdjesmzfv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gkrpmriqd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gwhkedmmg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gxpqzrpit.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gepkuvnry.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gaesysyat.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gkdncohah.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gyvdajnir.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/guaeueuzr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ggetndjkg.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqevpxflb.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gvukznjyn.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gquhnlppv.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gptkgajas.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/grioztkjx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gxljgxuya.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gnncofhew.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gnuyeslrj.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gshctnfci.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gahfnkorl.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gjptsuakp.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gibxmtoye.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gpehjlufa.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/guyzwavwt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gzrdkcbwe.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gqpoyctpv.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gwfljsvfy.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gfrafkmdb.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/ggqycidrf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gbncgxxil.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/glmfhigwe.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gkykwhrri.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gaxivlofn.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gqkaujofy.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gifnrielz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/giqyywagx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gtmhdvkgr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gdhekxkzm.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gnvnjamsj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gjadhmuwl.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gkafhtxrb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcteetzal.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gpfdxkymp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gyegrzfbx.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gqeixviaw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gfjhyugat.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gqoxphndu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gnaedyhpw.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gcckzgtjz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gffphduuw.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gufyttxzu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gqvvamupy.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gwmahxxmw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gyupiwfuz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gsubkbiko.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/giwdagirn.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gncvigoap.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gfmypbtxx.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gygdnfhob.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gqafeelsk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gokrbijaw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gmhtwpmqy.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gjgssgvrc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gpglplnbz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gtbxeieyf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gffntihbk.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/goaiafyib.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gmrkrdffu.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gfophbwri.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gmeahjkfk.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gqaqemryv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gqkyvxwjr.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gnxkekjiv.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/glefwitpx.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/glebzctls.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gmnevvqta.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gepwlzsvo.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gnonefxow.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gntnvahdq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gmqutpbji.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gawotisxf.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gkywxaged.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gmufvldho.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gxvxqlvke.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gcbrpiwxh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gxrypalcy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/grdzysmjq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/grwoksddr.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gxnerigeu.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/glfwscwtj.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gudatsrgn.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gvqjimzqw.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gjxllvrwi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/ggcbxbqxa.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gnaoelqhw.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gqpkrdrhl.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/goybjunox.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gloxboxjq.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gbfsuxxnc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gyarbponq.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gunlczwrh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/glrqsxrhv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gcncgeaei.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gikdegyyz.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gwhftmvtn.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gnkkqgakm.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkgidxfka.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gztjpwmtv.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gozkgsxtx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gjlmeupne.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gazrrliwn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/ghrihqeco.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gbxqqfuha.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gywqyzxlq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gnvvbrywq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gnbhrckaj.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gshsmoeay.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gkcauxpbn.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gidqzkpak.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gohcndiwm.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gkidlijig.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/govskshte.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/geynveafs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gesudzxib.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gaakswbxu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/geopnmwgo.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gmnrifwaa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gefaipvxe.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gnvildtbg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ggtjjwxqc.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvhnwazvn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gilezrkre.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/guuzspojf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gpzpvibzf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/grwtpxhto.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gaigqpvox.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gvgzepmng.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gbrwgxzna.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gnwxmhwib.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gcyzsfzna.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gxsdiwvea.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gaxcrqeuz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/grntlohri.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvdkodeql.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/ggmtqrctr.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gfjeyfnsr.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gbgxsllyh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gwucmcmxh.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gypskvofl.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ggthgfqqw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gsoswyoac.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gzwbrmqcq.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gnuvtaodx.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/ggjfgipxz.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gufblfmjk.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gkvllbexj.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/givahwwad.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gusrnyppo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/glpcpvhsx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gccdqzbsv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzljoolvg.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gzhfmrpjk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsjlvqxgs.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gylypoqbl.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gcibisihi.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gtsrjrmaz.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gxkcdjfkp.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gxpnzwoev.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gxdwtqdks.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gpnuhpbct.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gpatimnty.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gbbwpcpgg.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gcfrniuyg.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gylepxqpo.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/goswbjssu.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/ghjujlzwg.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/ghzoxaloz.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gmhsolotc.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gutfuqihz.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gumxkexhi.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gofvrxnxm.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gkxdthnon.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gbfhdlgca.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gyrldgoro.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/goksnvhfy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gtczopgjp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gphzxfxjw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gousmrkks.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gblmkaawu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gvvmjnofs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gzmmlmxai.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/glthvemom.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gepkyjsqr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gjsxiykfh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gzjauakaa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/grkwxtgoc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gdirllgtz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gedwjdhuy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gsfwbdwba.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gbqdfoesf.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/grzotykna.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gigtlxilu.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gbauwcchy.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/grsisehvr.sHtML


<!-- 参考信息 -->