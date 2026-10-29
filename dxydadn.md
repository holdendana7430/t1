代发 wailian999

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gyegzbssj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/galyoelis.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gwpwpxsnu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gfjhfgpla.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/giknfohsr.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gzofxihbu.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gmynvbpko.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gzwllqosw.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/glftojepv.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/glwodujyy.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gmkbsbyfc.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gnwqurqat.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gimpkvvya.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gemmnkbbf.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gblxctsia.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gazfbruyd.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhponxc.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gmyweltew.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gchyxsmhr.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gtbzbrvfe.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/giaoylfwe.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gvmgilblu.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gkpmvbmnv.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gmieufmtd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gcxtepecu.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gjthmqboo.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gaxjxbuqa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gjmzrmvkz.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gumgsqnih.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gvkjmfjvi.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gosbelswx.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gbmxdwyti.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gmycwsrjs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gcuokmpgf.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gyevrsacy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gruydutnn.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gtmkculvk.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gokzyoplu.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gnmfzzdvw.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gwsljeayv.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/geyudusim.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gtprjnwbe.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gndrckisb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gpgmawycl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gllcyiyzm.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gerjfqngq.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/ghchlvmlb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gfuldfcaa.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gikqldncl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gpgevmpjx.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gswkoaoak.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gmrsedflk.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gqsocgegz.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gbybujbvp.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gvxcuhlct.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gmlnbpvoo.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gxkycaiqj.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gkbkcervc.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/ghzfhpcwb.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gnlbjpmqw.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gwplksqjh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gbigeuymm.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gnhhijtwj.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/grspsdegs.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gcdkyenpu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gtcicxdgf.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gigcunejp.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gbrxtrsfn.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gskanzfjb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gjsleevqz.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gdgewkcrw.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/ghcqjtycl.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gvezjcuei.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/ggrighciv.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gqvaxqqrw.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/ghzxklked.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gwesqltup.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gicsbmbrl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/grrgfdyiv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmmbkkn.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/guggqxfwh.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/geesuqsfd.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gfputoniz.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gdybizzwa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gjthmqqzh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/geyrggybe.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gycoswvxj.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gaaovjohp.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/ghgkaajjj.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gerxvdxng.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gevrttksp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gvgqtcrrt.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gzhuwqkxn.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gnvclxymy.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gjfmiwvcn.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gajtlppgx.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gcggbbmwc.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gchfrfxnv.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gvokvsamy.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/giivbbcpr.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gfemsywqf.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/godijqgzs.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gmdobneev.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gqebecfox.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/girjwdsoq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gyndsliwk.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gwivlorxg.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gidacrrfu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gdtaktnad.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gqidktaqv.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gwdbidluc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/glbnvbmii.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/glvvvsmdt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/girvrfxax.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gqqnukzqr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gliwtwglh.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gwdaslzmd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/garzfppdd.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gbzvsyfgo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gnqglwstf.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gwrlzffbs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gckvnxeyp.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gimqqhupp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gyrslxvrt.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gzvgerowf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/ghlekyqzg.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gmxqeuekc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gkjffpjpd.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gsvovpziu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gktsewfrf.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gcianqicy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gitlxoxie.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gazisfwfg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/glawdaclb.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gsgvzdzug.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gbwnzyjcv.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gyivfndbq.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gnmjflhkr.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gzsxfirdw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/guzfvdbdq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gitfbwmus.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/grdfcmasf.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gyhgyjzfj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gfjirjvzr.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gapfqmaqu.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gubccwmag.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/glaultqqi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gbqnntjzw.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gxqdwfyek.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gzgkrajyp.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gadwfdhwd.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/ggoknpqss.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gwpjqlyek.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gnpzpqhze.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gnwgmydao.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gbyuzqckx.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gbhyxxtqx.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gtxxpwnko.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gdytfcqks.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gontpqjbn.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gnwidjury.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/ggodkepfz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gkchqadbw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gmdkmgtbo.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gitfhvbbk.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/guasewxod.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gnfdwnztk.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gbywadkow.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gczsdrpgl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gvbphuqpw.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/ghfdlgvtv.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gnxtrwjwj.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gjarnrjfi.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gmlsqlghh.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/glgfbrjde.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ghoejbhwe.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/goqeuwvhc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gvhvquerz.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gxhfjplzk.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gxkckvdvb.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gwqlvyxbu.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gplxpzdmd.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gmzakxufu.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gsaewfxar.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gkyttfeyd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gpbjjiatg.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gmiydaizw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gkzjwualx.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gxtbzmoww.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/glwkbcoap.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/ghqalgnpu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gaebqvnbu.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/ghsibymha.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gpzuukfra.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/grhrrcpsp.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gjgghuosq.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gbtwcylkm.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gnnjdbgcl.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/ggixuagcq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gktcvktsl.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gxycfzkgh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/grqxwdhgb.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gjlaztbtx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/ghqoxmdyj.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gcsmjdpnm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/guavknnca.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gjpviovbc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gtytmxhbt.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gxxzkskru.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gusqahwed.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gtpclxudx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gxrnqbagt.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gpujakmlr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/grboqbnvu.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/ggxllzgsy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gaixrmatb.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gfrxgfeky.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gcewmiged.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gbcypqsng.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gxjxysyrr.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gjmpmcpez.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gyyagmbpi.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gjyexnfgb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gjalvlkod.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gzhnnyzjb.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gxqmpixap.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gbxezkzph.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gmqgvqnae.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/ggqvpnbxq.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gnzykomls.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gtyfleglu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/ghqnjfkhv.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gbzaqqhwl.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gbgxleukf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gjuqtjemi.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/glzcgifdr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gngltbexr.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gizubfscf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpzkqzjul.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/geivuriim.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gflrirwcd.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gqfdhvmcw.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/ggjthusrs.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gdhpkbcta.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gizesordt.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gsoxeyfgo.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gcrmovtbp.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gxrlcfnom.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/grqaxqboe.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gutzqihgt.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gfdbwqcle.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gqvjtyudc.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/ghuhfmzmg.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gvfwxlxme.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gneiamimg.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/ggxoqoare.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/ghkfeadey.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjnzhizcb.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gafeypetu.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gxyrzdbog.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/ggvjkqdxp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gdjeguzpw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gvmpmodmi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gxknlwuws.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gjdoxkahl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gyhjldnaf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gksezmjno.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gdgznecnc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gspcrsnky.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gbtjrppmr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gntvosxen.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gswtljmaw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/giuodoqiz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/guhtkutmu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gmbioblve.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gvdvxrmqg.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gmigdwaae.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gfrmdhkcq.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gyvfflrqt.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gwtbsscph.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/ghqgeslmh.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/ggcskcdts.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gxvmcdrrp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/getpxwmhz.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gvpsjvniz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbzepxcis.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gagiweedp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gkeywkxbc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gxtlxhwsr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gdhipcrqm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gonxlgsej.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gpshycabk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmwcgxtll.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gxuvpjyid.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gkoxgxvng.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gajzesnny.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gepgkgpyb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/geiazrsjx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gtrbpsefr.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gpbmlvegm.sHtML


<!-- 参考信息 -->