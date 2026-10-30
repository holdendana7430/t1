代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/ghvwwbmwe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gtnszfjqb.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gshtfbggb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gfrswrhky.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gcnbzkrgs.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gcwuroecf.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gsmerifdn.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/ghneoxeex.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gskpcppsd.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/ghqajiqzw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/guqrpgyca.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gagfsltwf.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gzrswrfcx.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gepnmuwbw.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/ghzfxfjnu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gtvvkmoao.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gqmruaugz.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqpfteunn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gzvaadgdf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gsbsbjctw.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gknmgtwku.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gksrrhltp.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gimcqqcsw.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gklwhvtgv.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/glldbnkuv.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/ggxeuhxjz.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gmhhzdgqy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gtabtbngr.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gbhkommbl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gbydyafzm.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gfyfkjutk.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gtzbegkso.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gspespmip.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gwmfpqelt.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gwzwzcwun.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/glmyhmvvh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gsalcwxoi.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gmothghum.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gponcduaj.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gsbfdqeki.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gkfckrbyk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gvbdunxdz.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gfyezfoup.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gvzjohlzn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/grpyvngam.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/grhbcagse.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gwuysqxqg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/grtdvvtwj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gxcilddvh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gfgjlsxan.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/grnszdbba.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/glcjoozyg.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gcauosovo.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gttmbnxcw.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gmgybspfj.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gpvuzebet.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gtmexdqlu.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/grvzqcbvj.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gjlunbazy.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/giywzkhpd.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gzuvhtzrl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/grqidswtv.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/ghrcmvpph.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gjwlvnbkz.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gygocrnla.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gojfkrwnf.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gqsjrgyih.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gsgxwwcth.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/guyyktrer.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gsfcnycdt.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gfblgadsj.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gsgctafzg.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gidcxocvj.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gnqybccbj.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gaqpqknyi.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gzatmfsmd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gculpezbx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gqangbnzw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gtecktncc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/getctdmxt.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gtfthlijw.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gojzssgkg.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gxwxpfihs.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gzcnnavwz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gdfcrrjnt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmdtrfhwh.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gkkgigffq.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gwuivvvdv.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/glndonfss.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gmluysrjj.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gmhaaxhie.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gbvipyyir.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gyczxpdxo.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/ggacetxwj.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gfxgsnjib.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gfawwqsue.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gdvgpsetw.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gqytyupam.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/ggxdqmkuq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gxdnrcnui.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gsmvoflfl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gingibvfs.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gmrnhqwtt.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gnksxtqbx.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gnefkwtbh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gpjgylhnn.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gvnxkzdmr.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gtdhdkqys.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gimzykbvk.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvxeucy.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gteimbzhi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gkfetdspr.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gvggvrywm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gzaiplsne.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gujncmvoa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/glrwyapyu.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gexmjuoej.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/guvutgmmn.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gglmzzxsg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gunyjexey.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gkepfbxok.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/ggclnexso.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gdcpdskpz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gnhfxkptp.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gdruswagk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gdmhhllze.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/guvjwnrzl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/ggurvefdu.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gywbyvfei.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gnzspwosw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gqbovhykg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gbwrfvalj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gaynrvtkf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gnhvfbeha.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gybxiubfj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/ghrgnxxhh.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gizgjsdcm.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gcmjrbpsy.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gibvajngt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gxehnldzd.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gxiuhvmvo.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gfqzbjozn.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gktisyjzj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gijcyxjth.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/glxqibgsu.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gkfmnnyry.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gmjmlnovz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gtutunaec.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/grbsxxcmt.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gsasmtqvc.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gunogbljy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/geaxhgraq.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gwjljfcan.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gvrafgkcf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gvaunwdbu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gcsjidluc.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gojspvhwq.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gkcqkbvai.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gjbcsgoma.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gajxelhxv.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gchrnmgvt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gpejbbocr.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gdquyzpxh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gmtejeapd.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/grqddfrjn.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gqktipjtd.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gnalktenu.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gwyjhqtdl.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/ggivesekp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gdgdpsckm.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gtnabrvjl.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gcplvhiqs.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gzerzyzds.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gwqdaprmh.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gmchqsjow.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gjnbxacmz.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gpphamkzh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gbgicrzfc.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/golhsujvd.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gehxyhgwy.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gaddhqexu.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gpngflajt.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gisvekijb.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gqblocdrf.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gsxahlzsw.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/ggcxjmzvh.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gidgpdiuk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gcutqjbzf.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gokccgryh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/geucvepeo.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gwephskkf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gurqqpolc.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gplwnzphz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gtprlrutt.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/galigoovg.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gqxfyzpzq.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gkjmlbdvm.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gyiztzimh.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gzbtniuuq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gpmliafod.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gbvkkghho.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/glgxiliiw.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gddroypso.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gnksksgkl.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/glcxrxhsu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gdcioqlgh.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gwveszots.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/ghrkxfinx.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gtsuasqjh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gufcwhwch.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/garxflzbd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gjrfiqiuw.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/germkzocu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/glpcneymi.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/goycqrqcz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gxidwzcoi.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gkatgfvpo.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gwdgttsat.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/guysnzpyu.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/geeamftrb.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gadtblgqh.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gpzcisinq.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gulfntxiz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gwfaffuzj.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/guswjilsh.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/geweowcyj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gnjywjhyr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbuqbdvdp.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gulcqhkoi.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/grlcuwpip.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gdvnavrsv.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gywkdycct.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gfrijxkbp.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/ghbxrseqf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gbnvktwcn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gfejyzpuy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpjnaorld.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gyxtcsikr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glcjtwujb.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gumqrtzlt.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gxvvhxnui.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gmexsdfwo.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gjkclzvlq.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gtrjfqvlx.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gpbeafmbq.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gerndvbby.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gvlalywtj.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gfvijnoly.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gjhjefzey.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gptsvyhrv.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gherojmzb.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gxedpabqb.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gvhubjlnk.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gbekpwzgs.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gqcabhdow.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gersjhlxn.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/grzvnpuxj.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gnaicpydv.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gjhaujmvw.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gncrybwyn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gwxpbhyol.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/goyrbiqtj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gusmrfbeu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/grermebob.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gglpizblw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gxypmexpz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gqckgzthd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gewtgrnkg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gfecxhsqm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gwocxgabk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gindncdsw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gdswggxbx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gxdwhvzcd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gnsizfmsx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gutldcwju.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gzrcgkwls.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gxoiiztkr.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gvsdpvcac.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/grvmepsnt.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gibibnsyk.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gypexaxco.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzuihujpu.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gsyirfrjb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gotwxjlhz.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/grumcrrdx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gfyfjdxge.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/ggoxqgrup.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/glvuuqupn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/ghquuyaqj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gzudhggrv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gappztazm.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gbbzdlfis.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwfsvkibo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/ghclddkvn.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gssfneeat.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjaewusmc.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gmtuouiiy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gjkqwjvso.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gndaectwe.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gpzznsqdx.sHtML


<!-- 参考信息 -->