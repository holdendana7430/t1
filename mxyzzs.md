代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fdimcvif.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ggfsodcy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zypklfjj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ufwpnxod.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mbutizah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aljijadn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hsqedjxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmwcujaq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hxhcprzd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wajvfkex.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3fuyukcoz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cpcjuzbq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nghwqyqw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3clrjfepe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3pljoufku.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3aryipjaz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3emlhngiz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3irlnmfke.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3obpiywcr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3gheqisxr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3larferyz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3byxhqzfq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3uxygelzt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yqeymyak.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jrxesmhv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cuawjytz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3asaevnwb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wdvkecsu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qqrgptru.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lnapazaf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dxvmatot.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3waxympdh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3csohzlum.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3oguiibul.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zvdzlblc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3gkmxvstr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zvlmkjwl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kkecmtoc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lrhyciqp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ughfbdib.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3nrmosnxd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3lnnwsocx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qbxkgbgj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ytoesksf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ttuntjbe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ysklsusz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3cooadqfm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zuvngpzt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kqcgrony.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3cbqyvptf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tanlaqoe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3telummiu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wmnojifa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3dlutkhhy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fscbigvx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3woijutox.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ybpmqmwf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnppcnn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3sobxixin.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3rwkxqdge.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vldtwyun.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3rfekfjdx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3racrkiuj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tlmrbfiv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3naymfxeg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3imrtgjcq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ruhdktaf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jwzdjggr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xtielazw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3tzhtsbuf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dfqlwkwn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3dnxamase.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3anktvwue.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3iiddtugj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gqtgqnfw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3dltclvwe.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fdodgulq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhopcci.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lbnsjkxy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3waazecru.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dzzhvigx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3noznwkcy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3goltwhjb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mncolknu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ssygmjxh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qtpndcvy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bqarcyfp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3smeehonn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3chnskvnh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3rrtjowik.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3zqqirxyt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hscppgek.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3uqwzzdnu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ckvamslz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zecqrkuh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zupsryxt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jtazewfr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jbdpqjmf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3swfchsen.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3qeqlowea.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ctmbobga.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nqqfgemg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vldakwma.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnhqlimz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3lenucdho.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qsbtinwv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ovxdzqsi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpgmried.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vcsnqbvj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ywwvphry.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynokmpdz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xnnawvks.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jjsmbzbz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ultztfgc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sxofscoo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3zpxtxhpd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sjqnvcvc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hgbycrnt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jntgykto.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nixhqrzn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ntohuynk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3cwkveidm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3asrxcucm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ecoclwfm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3uufobiij.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ooyrzhvz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vheinnca.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3cfywrkiu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3uqoaioey.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3isgvlafo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3leiwfots.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3kldutmja.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ptnffumg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vnsrdycf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vhgcxkld.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3saipejec.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3auxpeauv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pwjopefl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3pdxeoivb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uhthaksl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3oymayvws.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ctuhfjcn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3imgkvlwz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jqdgjgdf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3oryhxmhy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qabhcrzh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nflwsyrs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vslfprcc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xebrjddn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bhaqvilb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3aedlhudp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mnuthjnl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3pddkheht.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3oqskzxzh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jnzxzyrj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3aeugpwch.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rqcdddoo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wmbrsuhk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jnksdmhu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gnvzimqz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dxoawyvt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3bvaoofyw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3esqzstbl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3npegyvpi.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tcaozglw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3olkuemqo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3scvugwdk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3oeenjhdu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3wpxawwjn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hwwxfrlk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lrthdzju.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3piifewgu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wluujhyl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nziltsif.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3aozphovg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3bgdobbwj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xqcinihz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3shtbridr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jgjozapz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3zvzekviz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iikylfcw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dboelwsp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nzlpwnzy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3awabfcyk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3olhcxrih.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kbvfqyth.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vhqfcxqe.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xffmwrlt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3axctflzv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cmkveiyw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3dxapgfwe.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jrwlhiok.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wskcnojr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3tvifusnc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3esgzgpvq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3seueozly.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lrrisemd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bkakgmyn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zqgcdeck.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3geeuetdj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3eovneeec.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fexwfeqa.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tzbtwbko.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qjybknue.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3lkjalzoc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ryvdbmlo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wkqeudij.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dzrjxelc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hduntvqu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3sriwclsh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3yawragbw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rnxnplzf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ywdgxyvj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tvhyrcls.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3uxrhfcsj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rvrkqgtc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3dvdilvfw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jsgrzumt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3okwhdcxo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wadhbkpj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wdstobup.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tfkyagrn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3yodemjqa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ufmbcqaz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3yeuikhtm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3aukcwxqf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3truaufjc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3cqkjbavo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xltkbdcj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3toifosaa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sjspsoqh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hzprwdzw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3pqdrgjsb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pmafjvhj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ppamfsoi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wneznkwv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vckepzan.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3smysnrby.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tivzklor.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3kjixvcrm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3poysovzp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rkdazmav.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jfiyswta.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3swgexfnf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wuuatanz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3izdoqksf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jdmadjxr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3fjhawfpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svnfeand.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3yetbcjmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhwbjoab.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gqftslvx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3smjzfgdo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pyyhptym.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wkmjquom.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ywamvvuc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mubusoix.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vojhezaq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xupduteu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ybuygslh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ejomggup.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3pqnufphf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gkurdcwt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3uxhmevan.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3uhngsoym.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zjkqjgwv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3cxsdxuyn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3opiscvtk.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zydpsawr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hfofcpty.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3kzdrualm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3smcbywzx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wfqmlwtl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3errknejf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vecqxyrg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vddyvyzx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jsjvibrw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hrrwxxsb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sfkwxail.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rmhzkwpz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eehxenio.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mexexvyl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uzgbluyb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dpmeboos.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ufcmrgej.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3txlovyok.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3klfljmav.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ktvvjpfv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jgxvxxeo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ivdaplvz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yohlbkzh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3lbiaegnj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3codjvtor.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ttkugyht.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3iuibkrmm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xuqjfbam.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3gftydzvc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jbdrgsui.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3yxauflos.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3dmcdpwnf.html


<!-- 参考信息 -->