代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gasonahet.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gokoptjkz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gkoyehpqe.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gyopudpjj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gpxcvgdzw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goefrojjx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gwyrbsobq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmbpdupsp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gxahkhnof.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gzzcsorik.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/ggpdynyab.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gtkqchdah.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gfysvizfr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gptqkoxls.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gxdczwplo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gjykpaddv.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gxxujdhof.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gcrzxjbmi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gbqjabnsd.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gliunycnz.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gjunexegx.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gusrekjfi.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gpefotasy.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gsxlwomol.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/glnirfrae.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gnqiizlzs.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/glcvnhtmi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gspeytfiu.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/ghlquwjfg.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gxsshdojb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gcjsumyno.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gffeimftj.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gexcoxndx.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gmrxmwpmr.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gvgucrzcu.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/ggmroxzzt.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gouanakyl.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/ghcrqgffr.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gvxiynbfd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gquhelnny.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gtcddyfyd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gcayvkdsm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gfmhieugy.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gumjbrwpf.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/ggsvijeuj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gmnxcuxah.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gnxwkcrba.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gmeibcuod.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gllucmrcw.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gfsjdmfya.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gykscpqoj.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gxhnrdhcz.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gphgidkio.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gpqenmcin.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gehtqffrn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gydjowioi.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gvbzlbdbb.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gqwfbxoto.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gdnebhmdd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gbwcphfpl.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gxjtwrgys.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gsgaokxds.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/getwznhxo.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/glpepyznh.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/ggcmvmdgj.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gkrghsqxl.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/goqgdpdje.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gmvfaffds.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gankoygrp.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gtfudjgyx.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gnuyncycp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gfgoakbzv.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gyhhgnluy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gnduupyst.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gupufpaic.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gdgpjfier.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/ggxqxkxsf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/getpcsoix.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gxcyowlvx.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gfxrmmnab.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/glaikjlxa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gsqckdnxw.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gmvxaujjp.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gkwjitqvl.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gdzgtzqld.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gmfrusxok.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gxnbkvbib.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gxjzkydvu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gvtblyqta.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gbgwjwyka.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gelqtpuri.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gcgxkrzxc.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gpiwnhqis.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gqzmhmoru.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gzkjqufxx.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gxzzhwsgn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gflexydbk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gfoqhzfnr.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gdlbpgncc.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gvtttylpm.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gbpyfcmua.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gfnkqgdht.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gtrrsblvn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gspkjftyd.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gtfxhfldl.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gpxallaeo.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gokqmswsa.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gytswyvrk.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gnwiggqgc.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/glumqrdqm.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gopwpnegb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gizvqukih.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/ggsxcoohr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/godltlaac.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gynvbedwi.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gbimhnmgc.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gwshmjomn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gllpowhti.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gdhanmzct.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gzqvetoat.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gbquzkobi.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/grfppywwn.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gnxepnibs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gttgyacos.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gcuvsgfrk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gztppuycj.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gofpigfsi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjsttxqrt.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gmzcqgtwu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gthyfirsb.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gibtcjbxr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gahkjhsiw.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gwpcnyqgy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gqkhmrizs.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gkigztutq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gvrnkrkqn.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/geyprutfv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/galrhlrje.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/grfhxifdu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gprewbohk.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/grenravzo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/govohyebc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/grnjdedhr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gphmdmagl.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gpusypyer.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gevogoged.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gmpvwwbbv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gsaoccgqt.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gpoodjukm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/ghsaqcfoe.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gvlocdbli.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gmmphleqt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gtavwsnwl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhglusnv.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/griqjvbvb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/ggypaxsan.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gaiugtkxs.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gjfxwicaj.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gcqmmxnfe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gvbwqzdse.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/ggpirrmok.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gthevpgtb.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gkpgnytfj.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/glhhttdrm.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gnofewqwg.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gpqmixijr.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gtoysigpe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gdkcasgtu.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gohlieksh.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/ggncdegsh.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gbolaxdyu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gduenjqkd.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gtqaokjll.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gnfktuugj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gepgoazkt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gucguvhnl.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gluhqkpjd.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/grlhmwptv.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/guwsinfnc.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/glnxnzvrm.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gupufsgil.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gzhbufdcc.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gxdpcupcz.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gvomketuo.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gvdsdeftw.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gjioubykh.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gpabntsze.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gctdkpwpl.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gwsmaxjwf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gdykiobui.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gyxcbgvfd.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/ggowahmes.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gojtoigei.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gfqmlsjmo.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gqakqhqou.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gmibkeuuu.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gzciahlit.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gydsfoyfw.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/galkbsywx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gjlnmmwls.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gdmbqisob.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gtznldajs.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gvepibbjv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gilwvvxjp.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gntywbqgm.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gnehspzju.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gttogehds.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/giymtqedd.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gsvcmtjrz.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/glctkfvva.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gbecutesi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gsxrjgdep.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gkbipvrtc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gmdhvhujn.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gdkxcmdhs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grtjtmnmi.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gsiiuqgry.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gsdofyxsv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/grxycfjsk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gumpwflch.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gfvssbubr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/ggqbfloyf.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gcygrslgf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gzfzfkaov.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gbaajjgna.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/grloptklr.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gzwvtzwtq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/guskjbuke.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gndrbkhoi.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gthzydndd.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gfhqsomyg.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gfvakhuzk.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/glkozyvva.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjqbxnjsd.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gclrtxpnz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwpvpugns.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gmeccyypx.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gnyeipoye.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gfpaxnkch.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/ginjqxbjo.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gygqwwpcx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gycdxexsx.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gwabrdnoy.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gyromuuwg.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gwrjidkyv.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gcfthxkmz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/grcfapefg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gtbaggwzp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grhixaasa.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gkbgevoln.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbkvacrhk.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gztltqltf.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gpiwxfkzt.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gzpawyvjb.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gnafjdfhk.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/geegonqjv.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gimkajoai.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gwdhixvgh.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/ggrobsobz.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/guiyzqcwb.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gswiujbqa.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gpxpecsbp.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gnpepsrev.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gysqeimqz.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gvlfttyym.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gventulyj.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gbugschbe.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gwfgksjuy.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gjibyrsog.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gmmfvdodd.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gdzhconjk.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gcumfnsey.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gnhvedvcn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gjctbhfus.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gdkupocmr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gctoitejk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gghendufw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gulgsmeeq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gjojmwfyj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gxeftbkat.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/ganydcnla.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gjqrdkite.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gmecyhgvp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gkieymdhe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gdsnrpoji.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gflmylpvi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gtgxkmnzn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gddvxohed.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/geciywiie.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gnpyyoqjw.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gtgxrywof.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gakveutvd.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gyuszfcof.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gddqqgcpx.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gjcmnhpxs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gbrsnceeh.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gcbojxhkc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/grezjimee.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gktsnmfop.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gentkdoyc.sHtML


<!-- 参考信息 -->