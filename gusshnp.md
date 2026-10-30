代发 wailian999

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gizhhdyyb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gtfgsrawi.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gwukanbpm.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/goviwdhpw.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gcmqqyajx.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gobghupmz.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gkkogpuuz.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gsflpyqdi.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gfeptlqyd.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gselkmqyh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gkwpovgke.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/glpjhmpnt.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gcawmyvaz.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gyepthxpj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/ggiudhrcz.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/grfmiwtzj.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gpbuklsgk.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/ggqapremp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gbiaxbxbg.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gzdjimkcu.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gxpwoxofe.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gpkhkvknv.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gpvxotibc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gaaiqdaha.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gonabwusc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gyfuzmfji.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gjklowdrt.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/guwihvdxd.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/geuztggkx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gszzreghu.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gqaarxipy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gjwiixhwa.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gxaxnkxof.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/grwffjbgi.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gvmxosdid.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gfyujfzqx.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gczgwtgbr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gxizlvngw.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gmqhwtbry.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gadxnkcjf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/garbusjyn.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gfvqcjzuj.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gzrixpgzu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gbmvpejra.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gvlniswyc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/grawwicje.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/ggkhsbhkj.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gvfwcylbf.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gikfiqztk.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gnpaozgct.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gyjrubrmk.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gunpcafrf.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gbavdygox.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gperrspul.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gaauayckt.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/glatgmkyc.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gcsisxstc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gqnkvfxjm.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gdfaavmtg.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gewytbbzc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gevsyoqqm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/giydydfep.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/grwvxbvgz.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gfbicruzv.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gyfkrmwww.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gdaekfxwn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gsvyakoka.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/grflvtysd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gbswtbkca.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gymbersxq.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/ghnvxixlp.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gnbahihlx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gouakuldj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gxxphrzqv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gxytmiwps.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gemzyxnor.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gwoinuham.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/glqpqcbvp.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gjcrdbllq.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gzkostwxg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gyaumlefa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gqqkkpsjk.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/guyowxlhu.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gxbehiqgq.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gptymcghn.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gmxyiopbx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gbcrqehem.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gnmiuefqt.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gvnsdbiub.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gnfrtukmo.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gymgeopzt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/genvbzpyb.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/glcxfwpvp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gicgdaiaf.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gosdliohz.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gagnbgzgu.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gkccggpuz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gpxfrwrxv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gjkdfwqeo.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/ggtltakur.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gvuyycfaa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gpiulmgch.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gnjdripsh.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gltweanes.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gyiinbmfk.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/guvrfugkc.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gejgelpxo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gvwizznlr.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/ggmssjiqt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gbchtvody.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gdunntmmg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gusgurjdc.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gkgrxprgk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/golkukxlb.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gljbmohtn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gjrdglpit.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gqczwuwqk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gwpljujfx.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gacldyvsx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gmsdwnhrx.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gmljcuebc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghggdaecc.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gupzkjdsp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gdtjzdtov.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gllrmwtxq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gmxsuksvk.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gsinivhaj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gewjnlhek.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gcwtqqsho.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gjcfeckaa.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gllonbdhu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gugidegbu.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gbpgpehuw.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/glfaqvkmp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gijmptqzq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/grhevsdnv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gmrbkpbyo.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gnhwpvwrl.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gctbaxyfv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gtzcgzige.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gpxwowslo.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gzizlayhm.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gcpxunuyu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gggecqocu.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/glzdjbauc.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gulvpjlwn.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/ghpzzilgs.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gwonmocyt.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gekijqxkz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/ggvukgaea.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gaesvwdij.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gvcvzckxj.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/ghjifhkma.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gtveslpuz.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gmuovnqrm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gpkvhbnyp.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gxddnkrez.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gdouywoha.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gospstots.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gctfkgzku.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gvjtdmkye.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/ggopctygq.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gbyfpmefl.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gupiezhpt.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gevllbkiw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gljpogfyx.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gfqumtpgk.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gvkeskncw.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/glmnqwlcw.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gbymhqmki.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gfskumtfk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gplmiylsq.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gmcuqcqkc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gnncyyqbm.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gqrkrsiup.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmkazbrop.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gtwhshden.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gphgzdhwr.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gakfalmyz.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/giibmzfuv.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/ghekjzfbf.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/girpjkcsv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gjnpgpwdi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gryuyfqtn.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gmwmnrusq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ggdsaxabf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gbmwnkorx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gubzfsygh.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gghrpmyxc.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gbjubwodi.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gayasqzvz.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gopqakiuj.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gdymvigpm.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gcakxebry.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gpozwyqmv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gjxzudsrs.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gnvuuyqhl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gcvgfrecr.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gvdxnmczo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gbydbiwmd.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gmvvednrr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gifjeyedh.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gmdxidgqm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gyptwyxsf.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gchdkoaqh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/guvqhnpze.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gfhyygjbe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gsyscengj.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gemgrhrgf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gqgilwjcf.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/glardyguo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/glmhnnhgc.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gyzlweawa.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gjxwakagn.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gniazmulp.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gstbtmjkm.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gaibecdfm.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdyswnayq.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/ghfmronhk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gxckdoywx.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gykwfdhkc.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gnyhjklzd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gmlcjjqws.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gaaxrtdlj.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/ggawotlye.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/ghnkmgmbx.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gsrthhxer.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gpnmfubhi.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gsefuwaxc.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gxflnsvim.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/ghajxyvkj.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gakxrhsqf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdqwlhfmr.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gxjencrnv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggsitjdfb.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gledfubga.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gmewqamii.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gelxhewcz.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gxoozrtyn.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/goqrtwfsz.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gsgerfhyq.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gupvylcel.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/geuhmvewv.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gmlorlurb.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gbckflpso.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gsvhiputd.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gtgicwxpm.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gpwhcpxoj.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gcsyjxkzt.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gmaakvmql.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gusplvpop.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/grntvyfnr.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gyrvavccg.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gjhqbptgw.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gwytzfeem.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/godfsdbkw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gjlqwahaq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gcufvbszw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/giymecejs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gjiwzugxa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gwvnqlspt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/glomcuhqo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gxzpgokbc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/geuqehegf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gogpvzphm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/ggovzlweb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gocephrtq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxojeihhc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/goaavzmhl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gsdbyhlks.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gdpnikipg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/golmibllj.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gvhcefzpj.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gutbmmgsd.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gmhfzglid.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gnficccdv.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gzlfuuivg.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gmvtpjame.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gzillasat.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gmqzgtyua.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gwnzbeory.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/geljjfmyg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gtvnsbhmr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gouhynspz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gwclfvzuu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gizvsbaoc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gxfzguweh.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gbpnocqxi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwiewbyws.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gifrinmgq.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/guohichos.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvbzjftjx.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gkmredjkf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gqgvqffnw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/godtvsthd.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gcsikawpn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/grovorvbh.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gcvmbbawt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gjjyweojk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gfteeshra.sHtML


<!-- 参考信息 -->