代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fhhvmgwl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2imeoyctw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sqqemxol.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ebywbirz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yggxswsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxsjcscz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oisvbbir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuevdbfi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2coxutzgz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vwjxckug.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dhqwvnnr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2asvafxkp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2omcribkd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qtyyrfty.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2irmzatuf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kiwycnhx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2mvljicmh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aktxucxl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gtasvqbc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tijayvkh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2prazgeds.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2vfinjfqe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vdibfabg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hpgidakw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2acxtxubq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhbwruk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lgvhlzfs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2nxsmmtfg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2xktlpzaz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qhfutahn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2rxpgbtih.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ujiidvnq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2avsxuenq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tlcdsaid.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2irgvnfpu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yvngwyis.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2tvugkobh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ovukjnye.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zqsrukjt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bteliczb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2eiagmfny.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2raaqzayw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2aimflsia.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2grydjolz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2iehaeasu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2lykymykm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2cdvnxhmn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2uegjoogu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ywecyphw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qnxuuldn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ylyadzxl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2egfdxdgj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lflzlylh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2elienayu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vatsygzh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mbjtsyvr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2efuhbmho.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2blpjrydd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mapeyorz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2fwqwednr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2yoabtdpb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hoavqlaw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lqsybqoy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qlipjldb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ztpjhpgn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2glqusgnx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ltvahuqf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mjmxpeoi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nwwlualh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2auekfdmv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rdgwvurg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2yejmpsci.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kvhyooio.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2cfssijtv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2gykshumn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2nwsumyqu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ffasdeli.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtkfefe.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hqhdxgdv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2dqzhtxxf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wjklciqf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tudenbvb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2netpvbzv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fxqigszm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vskwzzpa.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2zmxdatwt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gybvpwjl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ruywwsps.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2szlxmwwh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2inqmgqqn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dgpzbzae.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vlhcbodq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kjzudqpx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2aqrtktwg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2phhzapki.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2obimdqum.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mjtxbbwk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehmbiwji.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2efzktwac.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xkyczmpy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gtgdlvaz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2lwzdqymo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hgsslgbt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wywkwnhk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2awpjuehq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xmqcsuou.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2svbwjfkj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvytmpbo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dvybcjco.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jxpiqomc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndneolto.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2weflmbdd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hjcleaom.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ugmwbati.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2blpyshfg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2putccmns.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gozvaaen.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jlbrfqoq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xwuuaeqz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkqeoxjd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nievzjiw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wzjpmjwf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2evptpzjs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2anihmupj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jjhgbyba.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iggsmopn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ecnszcch.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2olvwcrlk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nydgwrwg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zzljcpzh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2vbguvwhu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ugxrsgmp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2zfbqhwnh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qocvqifv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2wuisewac.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bqlzsroz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2hccyjdse.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ahjkizwm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2svlsqfeg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2svwkohfl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ecpanstx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ldqudiws.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2tbvzxryo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dyjswwmv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2zwmpowoz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2wrzvdrsa.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vtonusfw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2euywfbzv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jukguhwx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2dfxtoils.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zuuelnyk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vmvmriae.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ioslgdma.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rayembss.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ocdnyxsa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ugkronym.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2lmkudomm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ifvmavnk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dwpixklk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ixohxjlw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fyisapuw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2huyuixpm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2npqcvvdf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2rekxzmtm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2vihoeuhn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2luceawin.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2uaynzwnl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tzcwyqez.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2mdprggtj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2tsbiqzkd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2eluskewl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2cxvkjkik.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rbdgygac.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2oihkziyu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2gufnrohw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bfaisovt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2kvxohnvc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ljmqtrce.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ipapghwi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2sllbsumw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sbbcnehc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qbnndkcz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2midliafn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nrvkzlom.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vtksbyed.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2prarvqsq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zcschqxa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltqpcort.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2yngjpdyg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2inezjlav.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2duusguke.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lvqwsxku.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nfokdark.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tjuthagw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kcsjtaqk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tbrxinfb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hzbwvgyt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jrllybih.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2tfksvtmg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssbtilhm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2aiwodnmk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xxymjtgv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2zdjzsvri.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xtlbxvvw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vmpdauzf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2imxiddot.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rsfcuxrb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2zxesawkf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2phtkykqt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xyalcrkm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mzchfoaj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vacdvihd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ybyjdhwt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cqmzaihm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2srsimgyd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fxbxyqol.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ihikorao.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nuaenwes.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nhaovomx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2pdvzeouo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2aignpqhd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lacazmnp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2seotgstw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vmofdzli.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wogqvjrb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dwlaliwp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ducbgpin.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bqtyrnhz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ftoysrrf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qchgalkk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2cxnehqud.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wlivuplv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xbirhupk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xbqnnqvc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2izeghmos.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jqeoqtsj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ljzfneig.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bcttnpjb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2leitxejf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2tkpekorq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2aiiczyzg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2rovrugze.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2cqnadjvi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2fraqmbxv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ovuszxpo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lvtdsoek.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jirspfnx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2xmmtreil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfdysrbc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2icaauzyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnrdubak.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jeqrzvqs.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lynympyy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2icuclivd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2uxmfcwjf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xsunyxau.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wwiisoty.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pqbzenyx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rnzuekvc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2njifknqw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vemaisuz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2juclmpnc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zxneyiab.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2eaeiraby.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jslzwkal.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2iygljdiy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qfzvsadz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2elfxfnzz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kdymyazi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yqyczgac.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2whoctqul.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2fczvreib.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2llcyhiko.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mfbkgkqy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2crckwfeq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ybylmnga.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hmprihgl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zwkckwyq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hrozwhoy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2akygnsns.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ifbracte.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sqireari.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nerdbetn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uvztawuw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dkmddcpb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2moggzatb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2krfgyyty.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2thzpldot.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ruqqfrhv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fzdfefvy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2jnzouwmc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zajjzspr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2gvcasshw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nsotlkzn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2srrrunpt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bqxclglo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ilmfunfz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kcuadiow.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2gglbkxzg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2yuivgbkt.html


<!-- 参考信息 -->