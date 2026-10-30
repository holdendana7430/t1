代发 wailian999

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbiajrns.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gjxkiqyba.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gemdvhbbt.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gdtdmmzkk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gqayzxvwq.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gxrlgiqoq.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrfnsejm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpevnrxr.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gncjgebek.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gafnhvvqh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gnehmkmxt.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/grmllefia.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/giixcmwph.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gddorxzph.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhzwdiod.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/guhkowzul.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqdjyeha.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gxjzrcmla.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/geyejkyef.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gqwetrqhw.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gbdojjvwx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/grefnfpfi.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gfkqzpkoa.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gnxblyktg.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpcxpsbi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/geffebqjs.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafidtvgs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaamldham.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gnxdupbad.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfdliqvp.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gsyifevqv.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/guxicfjta.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpwyoqzk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gmittygkk.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gyntxbbmo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ghnfnccrb.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gzicmqydd.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/ggwurkfkk.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbvijoyx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkodvvpuj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gboeqisbc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gdpxspyjd.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gmglgfdax.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gvaypvikd.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbfukffa.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxorlucuk.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimuulkeh.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwiezclv.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/golqagfwa.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gpeloyiwr.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/guqewyfgo.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gchmskshd.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gheyrmgxl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gfwrjnroz.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gydsarlmg.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhjcltti.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gonacueos.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gxsskgatp.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyagajhja.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gmboyuqex.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgvgnflw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeblvlhi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gbclwpwjt.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnkepjki.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gqztrfyhk.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gqyrkmldw.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gpuznbcqh.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfehdyhv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjkeshxr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/goxylcyra.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimonvhmz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gtvfvtpot.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gydxdjavq.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gexknqdfh.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gggxgpumg.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcabwvrzn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgmkhkpg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqdeybtve.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grkoxouuj.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkevgcvl.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqibwqjw.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gffowgvkt.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/grqcumnoq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwhrdecd.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/grvflwcgw.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gmkzjszhw.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gjzttlqpm.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmmgqvhfu.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golokggmw.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfarfxif.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyzbuhtc.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gsxpcjtkc.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmfxomx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/glcojoojb.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gyztcqyub.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gwrmzuwep.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gcenughla.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrvfyktd.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvamstba.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvummwedb.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/grouhnhtr.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gphbzxppb.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/guqpybvqw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujcwcypi.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gnucdfjmb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gizxpkwqy.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/goqqantmj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gdkuhgvcy.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gppkicdcs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjilxewdz.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gsudgurqt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegcsgoyv.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfuzffgu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/giqgwgfby.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gqyrszslb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkejybxhb.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwxcfygh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjwybdag.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxxlzohb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gjraxfyza.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/ghxcvogil.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gzdxpyxvm.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmwsbhre.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxzpraww.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/glopulrnc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gbaunfgro.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/guvwzprvp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gafsgwdbp.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfeqocck.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gobvvlere.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gcghvyjaf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gporhtxxq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlnuutey.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gngvfftwt.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzzqjvviy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjerjfcj.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/glgmvoezp.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrwugapk.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcqhdgyy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqsktumj.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gdlaoafvu.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnqbgprh.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgdhgrhn.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gmyirjhdp.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/glskrjwmq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpakotpa.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/goewwmghg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvxptqos.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gudsgmxzp.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgviyiti.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/ghreaapqd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gecepmupv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiolqdgx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gebwrnzsy.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gslmfxgve.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gcchtwrye.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjrbdnaj.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/guqidvpyz.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gagamrxvi.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gfoerlqyj.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwfmiyms.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gvvaareir.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gkiynjmkr.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtockbuap.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gvlgxvkrb.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/geoijinlh.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwxmjutu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/ghtsleoly.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gcuzffjfu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gmzhhitwa.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gemjpqjmm.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gndnyrjps.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gskxegdkk.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaxyffsp.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhmmskpk.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/grwtudhjb.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gjckpzzdy.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/glvqyfslj.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwuoblps.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfqxdjix.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwlgvzye.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcggqape.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxzcwhjt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gretspcto.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gtufuipiv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gyvadmida.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjlmgwom.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gemejpyul.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokwriaay.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gystybwvb.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzuxtsmc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoeufetn.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/ghncqngpk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gekztqnkj.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gwoeywqhv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gbasshdas.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gcsddxiwh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfuflexi.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gidvluhhg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsmvvzem.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gluzmxqdw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gciebfkoh.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofaescjr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgwwhrzx.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwbtzvvr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezvfbink.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gidnagwdt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gawpdpgml.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gndmdpngj.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbbxjaka.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gyznakvua.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkuakwsr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcypdgnx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcvcqgmn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/girfiaosr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gahwwjhxd.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/ghmmkyscp.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gznvdtrzc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gywfglusk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbegkgkp.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gmqmnthpu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcteximrb.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gywkwqiqu.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gegopfmle.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrzqbtzz.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsutgcnr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/geewapjyx.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlhsvnsd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpyguhca.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonuobzrm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbzgqbobh.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gpgdvhpbm.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gwqmamleh.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gglzafpkx.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/ggwlitrqd.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/guvjmareg.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gpichhtrg.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gvcyxeyqw.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaggdolr.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gzrczmwcm.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/ghnshlhja.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/grbaeagnk.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmzioete.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gghbelbxq.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkjnraoi.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigmbykak.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/graqaelvu.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhqgmneq.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gbkstokfh.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gvjnqfasg.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/ggopjhuee.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gawzlnyvg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gehomdqvz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gnummfdcc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwisqrsqs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfmimcse.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gxngxzyes.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaphkarz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gffdkygst.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gomsthgqp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gmtymupnt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gnqbfvzuu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gftavourt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfurgsbn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gjtnzqwaq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gyjqijigx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gkssaymfv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gxoxnbfak.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gbxbzoqpi.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcarmbpmt.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmcdimfu.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gopdlxruw.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gspzhdepd.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnlgisni.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gkivufkut.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ghsrfxnru.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gduaoiqbg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepkhszqw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gulgcvcsl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfpwavna.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gepscfpxm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gbldyokjr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmcqfajt.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/ghihhdnxs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygxpdknp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdstpdvn.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gjizrqwna.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grnbwfgiv.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gexrjqnye.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtilyfdj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpzphrpw.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/grrznockn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/giytjvxxv.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gxcxtzbex.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gadwwaipv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gucsaipbl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/ghiioxddr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gozakecdg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gappxgswx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzaivfpd.sHtML


<!-- 参考信息 -->