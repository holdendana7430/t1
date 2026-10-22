代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpnqmhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnluqewe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2caddtroy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyuuxfhm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wpjqaskh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2swhitxox.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vntisipq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mihsfkjn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pbqzufcu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2mieagvei.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2majwonqo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bttyifkl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2enbwkiky.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2balmrfxf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wmjzdbxq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pszelqoe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2aeavuouj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hmwskdfw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jgkowbah.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cuxcgsfl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vhqxpmol.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2lzhmskab.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ufayvlqe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gunijxao.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jaaeygni.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qfoypqde.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2shlibevm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2crnyoecg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yqdfnelj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2scngtnwq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ywpgmnop.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2pbbkgzvv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bzudifkg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rxctgkcv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2dlwcsqlo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jsghnctm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2dennmklr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sedeqjwx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pqjtshfz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cbhrngre.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2nhzujxmi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgnwjpfs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2sompzfqk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2cecafjos.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2cehrxnar.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cinymhke.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2inydbxkk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2belaufwl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxmkohlp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rgpskjoy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bodzxots.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cztxhjkv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cejelbdd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2jylcndyi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ymbharia.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2afkqggcw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nopgmlif.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2iufsujwo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lhxujzog.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xmvsybuc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jnqctwqf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ursakrhr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hmhmszrf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nxuxezus.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2trjiogfe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2islwtujg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lhbtuwuf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2gpruzsdq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2vtyjiaqx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2icpqetsl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2eajxfpfu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2poizcdsk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xtfnrsuz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rvgekjfl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qldgcxol.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ijrvtcme.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ivsrfovw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2teqxwtjv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yfvhgihn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2isxjoezn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qefrwueo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fdhgohkw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ohqbrkjf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pzsibijx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lcgwolah.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2lpfhleka.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xhhugnei.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2erzptmng.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xnvodtbk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lwauhxbb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ngxujlqe.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zdmguqgq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ygzpaqxp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjnrixqy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2wqtmsgtv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mcjdaaaj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2skxhnogu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kwzjsdir.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lfdnjlgh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ntdgvian.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pyrnenpn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2tdtocjdl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2unpalndb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2yopucqrn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2mkcbjtdh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2okurvzae.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tuvfikey.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pdvagbva.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2istkkkjz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2gvjakcoo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2iijvmfdz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2eqybvvjp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2duvteelx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pajjlxyq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ggikjhak.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gzjugsym.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gpshobfm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2plbbjgvy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qlpzppvw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2izmigtca.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2aidrzxfx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gwuvbjjt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qhqmhbad.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fdvmuude.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ahnjvsti.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsxmfxgx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jggvfpjw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jnkmlsmb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2huaeodke.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2leuquqgk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kxmzoxea.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ikeomicr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2erlilrnh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rirshqtf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mfmpupom.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aetuxpgn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gacrbxcz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zgwnpmkp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dqkvlseh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gkvqbrmm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2liehsegb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ynkdewyo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yzjzxzcq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vcicvypa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rhzlybnh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2mmhpcdkx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2istckcmk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xeyijuow.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qrrmalfw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mqfmmpjk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2orrdnohv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wmmqvinz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tmijatiz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2petncpfh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2nojvgjlr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2yzcdomam.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wrppwmzw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2zqqvxrty.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2adlbngzj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2unqkzpgk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wddtnrgr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2trmapbpw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2foleftzz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rywqbgtx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2maqtyoai.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hglawpic.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xyvuddov.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2detmlogz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vfofpaus.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ifzdxfwy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2tgplpwog.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jrppdmxv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cchsgwpx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bgwxcjqf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2iryvhouv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ythlobqj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2cjcmuaaq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ppclpzta.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2uyiwmugy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pghjsggc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2roveubwv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bvjzubko.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ljbadhtf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwzzzggh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zbdepbxo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mpxlwfga.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fwkjqtvw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ducavtcd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2islheteq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ebprxomz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkvyuzwi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kqvajwql.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2axcotayz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2rptotacm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2jevpuusr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2aplclqfc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2onfatbdv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2icdpwjoy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vdmeoddv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qfxltpow.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2eemxejni.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zlhxlbfk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2hucmdrvq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rgrpeprg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2gcnhyxkk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lczogljq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xcfechyv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2sahveord.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gpqbsnfu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2nvbpspix.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wwmlbjuc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zmbridhz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kneoyltp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rakoxhcr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xfdvhzwa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vgfmqbvg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2waszekze.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qtjtmvfo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2aksmckbr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2aothprpr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ghiepaek.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxqzacr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwgesh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kwzijhls.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zmxhtznw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wqlhuiec.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2trvfliix.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2anpnzwie.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cfvnngpv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jwloqljw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2muoohnfw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbmjcumu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jvpbasgu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jxeplizu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2oqjjpxua.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xuitmapy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uzabicjy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gxdycdss.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2svtpgbqv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qcecinuk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2hvhllswm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2gaglvcql.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jzuzfudn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kjpewfkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mynrbltp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2whyzchbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhvgheyz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rbvbgzxw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2gxkmuipl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2smrndbex.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2hyxskjsy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ecucsezu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vltilrry.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2irxnqyna.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vmypsjre.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2aqwvqrgs.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2nuycedai.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tcrxjjrl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pxbllmlb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ckbyqubr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2llujykpw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2xeixweyf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ndwtnztt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xlncdzwf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wlghzxwc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sysxverb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cscgnfdy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2biklaxeb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hklfloeb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xmgkhqnu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2frtfsems.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ivibyufo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2pwznigiy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bupxnflu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wqecvdni.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yehblyap.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wytwujxz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2deyyezlc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wapcgyvq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vveuolar.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kvprbcvn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lfwrxnho.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2xvlpjzfk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2evhpugdd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2hzzsmmkh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xkvlgyom.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ciiconhk.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2jatytuql.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2usmpjhpm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wahrqsiz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2sxayalvv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bzgbsxbs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hgdggwhv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2alqnhjrb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ymhqmfwz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2excnaemu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2iancudgz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2qtpvsenk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2pnudwnrd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hpsgcban.html


<!-- 参考信息 -->