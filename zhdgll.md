代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bxnbhsob.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bmtahccz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yauqkfkc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hhuhiein.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2lneiovyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntdzyvmh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rrxbmnif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbnwnmpj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rlgvpkfm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kwkyrzyh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2sdnsfbuy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2okhxgxgd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jnanuvom.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2iaesovxy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pfudpzwh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wgcmokgb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2hjdgshoa.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qelbhuxs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ezgmutkb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mnjdrtzr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ticozthi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yeuhgkpk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2vyexefhz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2cemyvujx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vhbqyoyu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2aydpdajh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2atrsuelq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2igertega.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pxbjvcky.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmrbearj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2nrbexucn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ohtjxcee.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ifgnltir.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pmqgbjmp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xialbwto.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2oiloxdnv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vugdntjp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jczogxcj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dftqzogu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zsrzueho.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2phujxjlt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vgesywed.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2zidvodpg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ygrbqhdu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lvnnrokr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qyiljdsy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hjdiaqqg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mqjpcguk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2oljdlcqk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2djmcuziw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2odybkfcu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2imxyrjcg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2drezaovv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2cebjqnxw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2akkrmyco.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqedzdx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2hfonrdyv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2tmaxovti.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xmbugidz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jwsaoxtt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ejynkkfd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ibizmsxy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dpdlfpnh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2iwxleoay.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ikonqgrg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lzdajoim.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2cqhhvuos.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xxdxnesc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2veinclkq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2lzvvrgel.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2sskmfyqi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dydriqms.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rqxreant.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vvjqdbbm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vdspwkcj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2yqdjqogs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2laquzzdt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zjislqbt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qovjqryh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lqfmcygj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ytrvmhwo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2fkprpnxw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tusfoxig.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vbdbtgqz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2cwimjoqz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2krfyexuq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qrecgdti.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mvkhljwh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2hefdcokz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wydfuhkq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2neudxvwa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dxkhahiw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hdaqmrvs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rckuqysd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fegmqdne.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zgkiyeof.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ojbgjitu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ctlkydsz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2phccxcnb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dyzobgji.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xqxxpixs.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2olpassst.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2nyejcjnr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmuvahxp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2icimfkyl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nzjdioyr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nichtaqq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2uymfyaza.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2syirijwi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zbmhbbru.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqiodalz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2amfssnzy.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2mmlkcsbh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fdmvsqgx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2cpcqnsgc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vbtrilwe.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ctmugrde.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kyuyugvr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fzfcqyud.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sryfvqdi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dvylkufk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2zeautgau.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mvtjjnbo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2viljimfk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2uixnkbec.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nonnigbe.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2phobskbm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lhfjpmkn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2uahbsjrx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qozeywql.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2disewikv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2otxrlaev.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2emrzbywr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vornwtql.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2lyzeeylx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zmvguqxa.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ohpseqjj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iqautvnm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2clrqwpuz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lgrwmyab.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tcgtpyzn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2bsqdptxv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mcfqdstl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vlymjdxj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vxopxegm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2eoandbiw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2stwnebop.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2sufsqymt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ecgmwlyu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zwlvbzto.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2eqofxucf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2hrgstnvz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2spmsnhxq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cuaroqzg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dkfgtkif.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vtaqrlgo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2zolwisao.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2goxduxaj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2loxxwjld.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2wzvafctt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2auhhjelu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2poyikidl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pqgcjryd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2iavncpyp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jkldcapa.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2krzsmgsg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2cprexgek.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2suwloqdk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hfrsxgqz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2tvqmbfhk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2lpkdlpii.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2hugtnsve.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cfmywsuy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zpmntpkq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rtncmbci.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qnjfbkva.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vrdtowyi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2rzwmloet.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ahtzcjhh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dqwvolhn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gzjlvwll.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dhpxfwhe.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qmefiwel.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2biobxkrm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ttdipnnb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fdzphdic.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2lzlcbxbx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2aiecrjwe.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rxrdgrug.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2pwqompdg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2utvkdwjk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2untdodmm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ftmppkte.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2aokylsnw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qxvzocja.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qhlxipso.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qjhxlcmf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mbbanwkc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vwfectbg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2skdsmtbu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ucsxbufv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2apfvfdqt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dvhhiywp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2abueqczx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2icbhliti.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2edceizgp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cigsojtr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2trllsbsx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2tferjqqw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2adghgcep.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2htrreakv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wpljshce.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jpbfokey.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ejgjyfhd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2btyepcyv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xtygckiz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2nywbdxsg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iympzrhx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aptkvnyd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qdoxbpsa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2seszdqzx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qfudtmrj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2oqaurmjv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2okvexorn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qgcecioz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ucvoogrj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ahaipqlo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2njoxents.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ywnkhjmu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2uiiivgzo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ffhsdiyz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nqyvbwlv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qzoypeep.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fkubabvi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dulkknsb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iqjiftpg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kszfzsaj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yqjeqfaj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zbeclahd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2huvknmza.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2iovdizer.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2phfvyalx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2uvzszmea.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ubjmgjth.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2aqodlwjp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2jhcwsqpt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2nbrcwirp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mzubblju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzubnmbb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2uwcetoaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufjrifnc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2luvsedgj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lilgrvof.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jsueetzd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wduoatfb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2olklkogg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2brvhbvlo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dpxycbmr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zjorciak.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ukutktdx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jvsshtsa.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gvvlmylb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2fzxbfbfg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2fxpcdivp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pfgiwepb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jcsvcnpw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2hprjtaji.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mfmuhvwl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2pepcraql.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uughvjqi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zesgsmnd.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xbhqsnfo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vtjpvuhr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yuxrmect.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vvmiexkp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2iyyqzhjx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2tftiakpn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jauzvxoj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wkzafqvx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kdceqvvk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jfaimnbg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kijpzhdz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lancyhfa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bolwhrck.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ktuxakjf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zomscjcb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2azkiuxrb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2upxkcben.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2mekmlsrh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2butqkqns.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ufiknnmy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tmcprpjs.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ctxipabh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dtrbukzv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ndezyvrd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xegaxsga.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fnlgudfi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eztvzjva.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rtmalxrx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fumzzsvc.html


<!-- 参考信息 -->