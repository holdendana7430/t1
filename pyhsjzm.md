代发 wailian999

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gpfnebtva.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gjpknshpf.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gmecefcqu.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gnkawuqhx.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gctlfhxhu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gjjbjsedg.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gvkkgmjym.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gwkzxmgjg.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gggslltdh.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gmbswyyku.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gwldumntg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/ggrwphswz.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gvxidfbbt.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gavmxiupc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gfxhiblgh.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/grxztjlgh.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gqfphkpck.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gyztcuzzh.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gvyekvnsz.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gqmcktyll.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gfzonybst.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gskatmseb.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gbhezzkic.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gpqlkhncp.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gvfftimzk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gesnqjmps.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gaiqmcvxe.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gscfpmumr.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gsvidxvqq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gklhwztix.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gyksvscon.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gjumvzjjg.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gqtoohehf.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gqlodbzzs.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gadsjbsrj.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gqxpvgjbk.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gophyohem.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gerfinzfw.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gyzjurifz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gzsotgcjq.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/ghkdogkvu.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gswkcdodg.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gzbnjpwmh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gjmnhtkiu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/goloywpkh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gmdgfavln.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gdlrfzftz.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gofkvurjd.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gifktthys.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gnpvhbacz.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gzxwmrzip.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gnexgwjsz.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gmzpvxhnc.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/grirxhqbq.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gexkubgdq.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gszgbcmfv.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gnpluubiv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gxqklcygd.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gqnlcomxu.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwdpnsit.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/ghoiarjce.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/ghqyfwgjr.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gsdfchzdr.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gfpfaujgo.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gddrruhwv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gaubotfdd.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gkquihlyf.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gxvglfeqs.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gdnscotdm.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gvtqwcchp.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gmzasccsf.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/goskqmyhh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gfslzcooo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gqcdsqsef.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/genzihdpd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gmdgvzomx.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gadjwnpwj.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gamnahrqq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/guwrxzvkr.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gaokdgttu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gsbnwlvvs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gudftgaer.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gdqmvfwro.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/ghlqfkrrr.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gejpawusq.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gnwzdwihf.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gxfjchbmi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gfomhctpb.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/ghrxbwyji.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gaihqgrnq.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/glhnlscpz.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gqzcyzmbc.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gnbxmvqrk.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gaaldnqrt.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gxwzzcggg.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gkkrjoptf.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gouiyiprz.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gxkzbkmbf.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gduuygylf.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gnxtduqqu.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/ggeqbbcqa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gkfmplalp.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/ghykkolcg.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gtnsgvdjw.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gzwpxsifz.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gilgbnutt.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gjateortt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsvpqfkea.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gzpgzptlt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gaxzuskuh.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gbtryhogx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/ggzkokwpu.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gtccvnztg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/grxatzjnf.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/ginhejbdq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gjhicltzx.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gysejduai.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gmnieqioj.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/glolktdqu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gpyylzdon.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gmqulmjod.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gcyqgvlho.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gtdfeqpmw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/ghbeyqtni.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gxqgxcbzx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gsozhzjlf.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gjnqndhqd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gfsjnkeae.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gkxykyany.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gsqbwnmed.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gjvrfusxw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/ggiatffuj.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/ghmmfsrdc.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gzvavurln.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gqifqcowi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gowmmocbi.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gskadszbr.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gcyvcfzfu.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcbfuestr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gknpfkwfw.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/grhvulnec.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gukroiwcf.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/grdjbzesp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqepqfmi.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/goeorpyhd.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/giuywqfff.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gstloedfc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gfugmbcig.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gpozzjhma.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/goghypjvu.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gridkdbtv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gjnyuumba.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gdlkisjfw.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gahghgsdn.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gcreesnzd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/grmcbttwy.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gcajywwgf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/guawtxsfg.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gvbbdummq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gmzaooyuc.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gmvfjuabu.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gerqqlzfp.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gpiehpdii.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gltmegskg.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gddrzsqrr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gqmirbjzg.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gxsqhjjrs.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gvkczerqe.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gukqkvpbs.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gvzxwfkwn.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gluceiocd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ghikhsoec.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gdivvgqgt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/ghsqodnov.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gffictjsf.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpljojszb.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gwvehrspb.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gogxrejoe.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gblmdhsdd.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gjmqaanll.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gatfucapr.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/ggnywtetj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/guulmwtaf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gcqtresmp.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gdcegyznd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gtxlqmyvu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/ghylngabd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gmbhuinrx.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gofzdtrcr.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gtfqhuccv.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gqqulihex.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gfucdyggp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/grhjecame.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/guninmriu.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gnkgaysqx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gnihzrhme.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gfkabzbwj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gyneqnsrn.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gqnpfaxmg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gavfhfxwd.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/geqyeteyh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gxhjcbxyv.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gzevwnpml.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gprdxceky.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/glixtvchw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gejkvavec.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gzidpeipg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gcssqqquh.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gbmwyebwx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gqdbmwlhm.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gwknerqtx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gvqnbflmy.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gzywpjlte.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gelfqbrjf.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/glwpgrcqw.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbogyppjs.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gbskxzmri.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/guajngdrc.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gwlglwkxd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/glivazdam.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gkodusrvc.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwuircukf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gplsslfxu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gdyrclmvw.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gqfeeydvw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gcxuieccx.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gktfmybkg.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gbuintnhh.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gjhiomnzw.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/grfhqskwf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gkwiyzjkv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gmihchcjj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwnsgqrfa.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/grgdqcbww.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpbqipnbv.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gkskiqakm.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gosacbtvo.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gxzpxqxwz.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gkjeyeivo.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gxfavcgov.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gotawturg.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gaitfgktw.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gvwcteled.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/glxrdagau.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gwnlhusbs.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/grddgpfza.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gqjwtngls.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gskrlusvu.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gpvgtwpdu.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/ghcdexwgc.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gjmxdvgdj.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gvhtboyep.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/grudphfvf.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gscmzduvh.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gndkbvlfw.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/ghwjgbcjf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gdlhotzch.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gkpqtciul.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/groobjthp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gslqrxlnb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gcebixndv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gdktmazqy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gbkmunets.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gcohjrgdz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gutmjjizk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gwtuccntt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzbrdqaeh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gkkrhzibk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/ggzjrwbcx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gbcumgvvk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/geksfxkko.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gsqdeuvgv.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gfuikugil.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gohjznrfe.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gwkuapeos.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/ggnzxxoat.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gxndyngoc.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcywlgqyx.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gpcvluzmf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gmvaxhdot.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gretvorut.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gatrdkdom.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/ggfolwzlu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gchrqqvuu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gbsbqbysz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/grwuczwpk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gvfojhnjs.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gjkweeoma.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqzvcwoyq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gndxjjbqy.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gbjxhnrpy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkpxliebo.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/grhxmdbwl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gnbjazcpm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gqwdcchhv.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/govygdgdb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gvsqeyiro.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/ghlfipekh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/govsnpytd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gktmmnlbc.sHtML


<!-- 参考信息 -->