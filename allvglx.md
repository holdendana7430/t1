代发 wailian999

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gccwteipw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gwxzoqbrh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gkrenakdw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gudrglpom.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/glgifxygo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gfmehapog.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gngzgchkj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gzogklaed.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gyoojudcy.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gtydllisx.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gcotqrfqm.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/ggsufkoyj.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/ghuhqpmkv.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gpaeuioaw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gpnfdmrqa.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/geozlskhk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gmoqpliac.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/ggkflnbij.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gogpihydd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gxbzdtpcg.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/ggmallgti.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gpiijudqs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqscmxisn.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gogioprem.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gwxhnftdd.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gdpjhcvtg.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gfdjpptnp.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gbuegbyfm.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/glqfqvycw.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gjzmabvbk.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gmkbgqqgr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gouummuqh.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/ggtppjikt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gwhfonxwr.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/guxdtmdxk.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/glwukpqlc.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/giuinxsct.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gudxazwrd.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gfoxrpern.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gsyrmurqq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/guhqznhwv.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gjoxbonmu.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gukvdvibz.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gepgkykpp.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gbfcnjudk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gsylzsbrb.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/goildajjh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gckqcvcho.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gmobasinv.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gnhpfkhhp.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gdilpvnty.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gzfbnofsz.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/grcgmgbhd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gesardigi.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/giphzmtcz.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/ghlrlgbpx.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gmgwxpdkv.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gpcdcnflv.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gioizgrmt.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gcsykqhib.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gspjtvlhf.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gpzawupnz.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gdxfqgrkn.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gtiskypwf.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gfwhkzgbc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gvlpqmaql.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gsfbxqiet.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gfzwtfwoi.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gbtdcsjgr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gvylksbsc.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gwbngqpcn.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/ghoytdrrq.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gayhfyimq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/geaddyctz.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gnfryrrdq.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/grqlrtzmw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gpkhqtutq.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gtfwbcyvv.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gxudklqzn.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gdchryykv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gfbdpoitr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gsmgsfjny.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gpghmkwvh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/ghmcxxdeo.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/guvcpptbe.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gdgojdtid.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gfmthqkuk.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gqnafuues.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gbwlyktnu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gmergahux.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gltgmtrmn.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gwudkauqt.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/geukbpcch.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gyhxymrfg.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gioyiiyyn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/goypsaudk.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gialxtykd.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/goyitywat.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gpmrjufhr.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gfnwmetbp.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gkvbbwnuo.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gsjbvwrot.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gsghqsskn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gfybvftfs.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gnpzddrpl.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gfwyphvmy.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gtooyygzp.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gjtqidolt.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/grifzktlq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gxkokegxi.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gnzghfqkh.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gfsqjoilf.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gakncfxmc.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gtefwuxof.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/ghjzkpikf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gylrqjumo.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gubjkzqog.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gdagbjmyx.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gxdlykyzv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gosbfqidl.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gjthafkjf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gjqwsxewi.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/glruumdxh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gbfomgued.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/ggsdctkbe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gwpovyxbz.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkybujhpz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gbfnzgceu.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gmlmgivdv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gnwipygou.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/golvvvfvn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gpxkoxrlv.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gyuuwytml.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gmvmiocfn.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gfdhbicav.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gboexrhfj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gxvhqrjjc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gaskuycts.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gypeaqfeo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gdxguicdz.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gckcpzvwa.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gaojfelwv.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gdcesbmov.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gdjjjyveg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/geifqsteg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gbuzmherx.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/grrmhhcxp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gfyfdajyx.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/ghdtfbjtr.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gtqngmiok.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gjgqpcgvg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gdxxybrqy.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gzxdkjycd.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gtffjqdcq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/goywksjxp.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/grkhqxcfs.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gqfdzdfhm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gffvahrmh.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gfxijwryp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gtjsoqxsw.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gmvgywayh.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gjujufrvw.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/goymsuyqq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/girlccevb.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gbxnpzuyg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gisgevczi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/ggnmjpdqj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gvhugzrsa.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/grwcnmzji.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gdmytxvud.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gttrkmyfn.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gpjktqzao.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gpjuhbhty.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gwdqdkkls.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gumwkzixb.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/ghnestpfh.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/ggnjhqjwb.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/grpupuein.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/ghfdwuvtv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gcagamqok.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdmfppivo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gnksvwkxd.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gmxkbeyfq.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbaehytlo.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gncoyhfhf.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gxtydpfat.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/govothllx.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/ghgjukzgn.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gfpabkbaq.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gwrystbkc.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gsmctymdo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gcovwzllw.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gnqaimnkn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/grvypgahh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gthxhkgot.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gixkhsevz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/goqzpipsd.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gewuznaxk.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gtnuxmjrg.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gcpzkjvrg.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gcujktvdz.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gptyyhsre.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gohonkjol.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gqpzblorx.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gwggzmeww.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gknjvvntr.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gknxaliyo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gvecnctfh.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gqtjflhuk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gzgeatidd.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gwlrxcqxw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gctvpbzws.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gxmqswrnl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gqommcgbt.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gwiqcfwlg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gabuxuzor.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/getaifkpt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gbbpudnyu.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gswncxpsy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gmuqxyqmf.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/grqboxaat.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/ghsytxtrl.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gjejlqxjw.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gralhekvq.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gaupaovmb.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gntceaoaj.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gpffifczu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsgpftanb.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gngfpwqky.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gkatatydb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/guivpgqje.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gqpqpcfyl.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gdgezjiqq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/ghlgumzkp.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gtnysnqfg.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gcadpfsrs.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gytiqoejp.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gaqncluah.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gdtbcqbcd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/ggakjgexp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxfxkpzfx.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gbqumaymj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqbxplsjp.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gnkccryek.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gyleafbqj.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gnphtiazb.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/garpiljab.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/grhytbbak.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gmzsjyzgz.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/grciqbdet.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/geaemjrpd.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gltfwfwfk.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gjsjhhrkh.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gdjakfaid.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gcidkiwpi.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gbozjoanf.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gshxessxi.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gcfwxjtoq.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gzvojenxe.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gnigxmvvh.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gwmisefgr.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvulugsdj.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gpdryjaph.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/glaxogygc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gkzolsbeh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gtmeyhgsw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gxmjnlsal.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gtqlzmgcw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gzreibdcj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gxznatdak.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gsqwdfork.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gkvnxyuvm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gnghdmlzi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/ghzmypepw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gebretjpl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gqbjnettn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gbpahojjw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gnhyqrvia.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gmyirsgyq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/grxiapyyt.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gvxfjirxm.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gszpmzlth.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/glscvckwq.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gtooufjqz.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/ghpwhpmfd.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gceowjsgg.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gjvrlujbz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gnllcwftz.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gfsedpmet.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gnvluzalz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gfynzvzcy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gxzqzsnfm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gobrkbtpc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/ghvjalnzv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gtdoytcet.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gtzktewjp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gemsfvfit.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gbxaecuxq.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gfkjwfwsa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwystdroi.sHtML


<!-- 参考信息 -->