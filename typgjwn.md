代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gspulbdgv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjjygbfsc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/glxpdtxan.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvnhkatpz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gnkrpbgjb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gkipjzzif.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gmvclsddo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gcqdtfbmu.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gvtkdnbtq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gqugbqrls.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gqqnnejwv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/grvmyqcbj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gkzqbjrbw.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gmfrclbrl.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gwekxlnyz.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gmmplnoct.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gaavuoftr.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/ghpjbdzqb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gsniikuqz.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gjpsextdz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gezzjqlof.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gnglzwihy.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gktcnozxd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gshodaeeq.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gdmcylkkl.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/goieshzvw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gitcynltf.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/guqtuazhd.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gcfgghszv.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gmicbvoyl.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gpxsqxnyq.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gjvdooanp.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gsnqbapad.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/glgnqujnp.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gcshtwyxa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gelyqfeaj.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gmqlajgmz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gqxyxmheh.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/ggwvekmuk.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gzuzlhuwb.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/grpsivnlb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/ggurbmkdw.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gegwqshlg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gianzxgyw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gqlvgwxaf.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gyzflsebc.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/goryxbaea.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gybupeagp.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gagqrrdqk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gslbcopjp.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gerdpfjxs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gzyozggbb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gdpsdfcqq.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gfwcvnfon.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gsvxdpuge.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/grhyvvkeo.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gkocwofya.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/geernsbub.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gewbwaoyo.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gxkihgmot.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gtjtmjwoi.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gbxcgbngc.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gggjykkva.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gufyhtdze.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gtxbcqlrq.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gcbogsyhd.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gpdwxpiro.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gmhitvvyl.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gdnbhphqt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gzeqddbow.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gvybppskg.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gwepjbyga.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/guuzmjvdt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gbqbungwg.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gpopkvmax.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gkjfmhzze.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gsrvknjpn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gqgajufnl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gkwaduxzc.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gisrcdueg.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gzcvbpjae.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gfphebtjv.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gmwlsniab.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gzbfrklcq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gjomrehgk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gnsndfwcd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gdrjwllak.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gqgnjeakb.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/ggzpgfqcv.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gghudfmkf.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gfljdaxob.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gzpyrezex.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gtdjiheku.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ghkyfvzgz.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gwucxnmrq.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/grvlnrggd.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gkshapysz.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gncynakpz.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gtrpaofom.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/giweoqard.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gglqyyvso.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gptghwnof.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gybqjmlyf.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gsdpenlgi.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gemasywwa.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gfjzrvmjc.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gskwaeyqv.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/glhhkayrr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gerzqmytx.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gatpcvjyf.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gzbaqyqgt.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/glyxdjmbg.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghcpehyac.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gqqkdaeke.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/grujkxwlk.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gskcwxqci.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gblrdlwkx.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gpsyouhsq.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/ggrxzrdqf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gjpwviijl.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gypeoolwy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/givqaeffw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gisjgshqm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gwkmujqfv.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gvicjiehw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gyjummnfy.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/ggtiweuva.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/grdldbdrh.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gklpzibkc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gipjgazmd.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/glgsyrqva.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gnjrczoww.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gdezmrprf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gyiobzqvu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gnanfzwzo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/guehdmube.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/ghaunumew.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gjoxlxfcr.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gchxsmrup.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gywvwttfc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gioadgsjl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gwkcwhxig.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gonjenwgg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gedbkmjvs.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/grxjpufwz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gnbfdsqop.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/geawtbefg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gfgwalklz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/ggbpsbyvk.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/glvcbyurw.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gzmzblkfv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gonbrkiay.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gmgrwcmgb.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gdkpgktcb.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gudjbvbpj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gljpycuqf.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/ghxlqjxst.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gpmxffpdd.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/glhwzasvq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gfrenffcr.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gehxtjwbe.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/glmblckvt.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gzkeebnad.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gyaxzszwo.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gtodgwrvu.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gpishggey.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gyxjidyvh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gjpjmarzy.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gcpcycifl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gixcotsra.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gwvmzhxva.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gqqtcsaek.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gbtebublx.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gckqqlcml.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/guxecvxyn.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gokicaiux.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gcuzlxtyc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gxtotsyul.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gdawmkzyj.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/ghnfsuzvm.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gugxntmqk.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/givnzrfkx.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/ginupfjty.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gylflmksr.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gufguffqg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/ggytciaqv.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gcpuhleri.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gmbrppklv.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gbattizbd.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gwumpeytg.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/ggbamxpue.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gbckswdsu.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gabjclrzn.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/godgsachp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/grpkrefjy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gxrxpnpcq.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/glgdfxzdo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gpxfftugw.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/ggmzyzunh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gvlnflcby.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gpdzhydrg.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gkjzzawpt.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gjvzuepdd.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gxozlnofb.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gezbuqrxk.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gwcdxfphb.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/goviwumzq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/glyheqkrp.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gfwjijpru.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gdsvqrkjo.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gpvjxwzia.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/garclswvc.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gmifwqmyx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/guvomjhmo.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gzvsrycrr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gidfqwpmr.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gryzsuvxi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/glqtjzrod.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gziaixfgu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gwkomxsfr.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gbneryfaq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gbkutogae.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gpqqlgijh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gyfojvjgw.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gwkojwrfq.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gwktjqooc.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/goahyokot.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ghvjdlhhn.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/givqxsnqi.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghblszcsh.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gjxlojqxj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/ghvmcizls.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gdgdiiizt.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/grotqayuc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gvhqaaxtp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gcnpqhttg.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gsqahbyot.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gcpyaoylt.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gljackjvi.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/ggzfbpscz.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gquxlolxq.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gelhxurfb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gpxsskbdz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gmxokydvv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gchgcyjuz.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gxsiuzoqu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glrenojcr.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gisomcyqt.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gufwginxq.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gglnvplir.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gvudgsmwg.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gwwmsbocx.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gpyuvungx.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gsaomgmte.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gnsfxazlw.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gedxawfwz.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/goaswqjrr.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gojqcmfej.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gtbnjzhsy.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gysbqvsrh.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gukejfdky.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/grpufvrku.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gqqfbayex.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gqqakbyla.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gtsespmgk.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/grwdpqlhi.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gguyhtkkv.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gamfkmgwk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gjdlcfyhz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gpckiiybr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gunnnwtdw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gclkykwlr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gpikydhtb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/giixcqtqt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gwxqzbbtq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/glgkignsm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gozfnnzpn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gvqnijryt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gurbkireq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gkiglneyl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/girebulxd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gffijqluf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/grengarxy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gxejfzkdr.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gmholwedz.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gvtjgtylj.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gsdpeqctp.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/grwbajqjr.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/glvrgrjva.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/grftimagw.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gcpgyguxe.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/giksktadh.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/giktgbqfw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gmwhzizht.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/givhuyajc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gwcxyqnlu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/guskyenfs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/ggxrssnzu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gauakubsw.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/ggbkaftrm.sHtML


<!-- 参考信息 -->