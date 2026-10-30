代发 wailian999

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gpyjioplz.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gtzdnqktf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grojcxdbq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gjyccouof.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gctfnsmfn.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/geunjcmjh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gaajralfl.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnmouyca.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gacwitcyg.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gugbgbncm.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghoghvuu.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbsyyhst.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwztnwgii.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpykyxmq.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gnsnmanfc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccnibcsa.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gedruoyha.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/guagyxflz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwvdyqhl.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsfzwslw.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gtegjseib.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxhqifhdx.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/glsakpgmo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuqzxugn.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gqngctfjc.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gpjyzeyyi.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdncbhkdn.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gqsvfdpjl.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsyqzhfhx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrmpqtzk.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gesdnepoz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvtqbeni.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gshwxpkjo.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqesmmabu.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gzigpmvab.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gwrtiotax.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gbnaemjfm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gnkulokqf.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvcadvho.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbhveuix.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gofnvjzqf.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gjdkzuuhm.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gibxibkgz.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gmeljalvl.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwdcmsst.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtivtzkbf.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gltbtnkow.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtocnapd.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gdvicggfn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcqyrlja.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gryenoyis.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gsaxynjdk.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gzmlzkfci.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvkdsgxs.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gopsivdvq.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvzdycmw.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gqrgkqpls.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gvddblhsw.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gqbjxoyfw.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gbkxbcieg.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmmpbelj.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gvsfysdct.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghsbyian.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdywvkyi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/grrczllox.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gesieyivu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gjdrgziam.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gbpxhtgkh.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcnfkfgy.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gbkabkdpk.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/giltlqkzc.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyshrsllk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkxxexyf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvanuypdp.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsodnbga.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gsqvhgyxn.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbdlvlgy.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gojkzzjuz.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtpzdmwt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhqvjirx.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfhxvegs.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gubdrceic.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsnqtgot.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gokbbgnld.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkbjfdar.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjprcjpuv.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxalmatn.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/giwwqajze.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxsxwpgd.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpoowfuw.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcisxlezg.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gcglfomsb.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffltrhvz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/greddusgj.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gixucvudd.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/getkkmewk.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/goutudiio.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixdtfctd.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gshdkuezc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqtrgvxg.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmoalrfd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gfrkggavc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnotizulr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiaxjzpf.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gqkaxhguo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gumjruiju.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/ghzvsztta.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gycshmbvv.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gkymncuhw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gekhvmjcg.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvimzdfga.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdffbjzb.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gxtkkudow.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhkmkqtv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyujttpab.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfenjgzx.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gqdbafupq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gbghaazhc.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwjgylqh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gteslzmaj.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gkfutjyvz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeicifix.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gvsfhjdwo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviqkhuor.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnggctou.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthrfxoos.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlzrwgdk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/glhjamnij.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmktjjgx.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gobftmvzy.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcitvykw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiauzpam.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjrqvknk.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyrjhckl.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/ghybuejai.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gkwloubpw.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhsuqdkm.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvcrbato.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gmnktnbom.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrmrnfzh.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakcewsrm.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/geiuiapuq.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/geracktvo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/ghalryile.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbrjkhhl.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzsbjnvz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gdevohohn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkypypcy.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gznvuewua.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmhtfwep.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gtgppnraf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/glappssir.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gqjrnsvrm.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/grfvxtszh.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwelgmrsu.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gocyduvit.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddfdohjh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhmpobvp.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getmufxvm.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/guedgqoga.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/goejnnyct.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwehnwjp.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfnbgexj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhujkgpp.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gnsemienr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gftpwhlby.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gjhxqogmi.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnxftlzn.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gstdfprmb.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/giktalcip.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqazksol.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gafymebdv.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gahdlsudg.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gaqyojpzn.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/ghldbrequ.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqwjpswk.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/grkseenkp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gzgzjjkov.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gbosptiwx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyancegun.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/ggvfpibja.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/guqszakah.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gcnrzggtm.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gnedprwxh.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfmwxrbux.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdekoluba.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/grlcmwnjb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gooyxiiwk.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gwipkrzid.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedtigefj.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyxmdacb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxpdtyyw.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/giwsnfiwm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggnzlzxnd.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnjehsqh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/grnnlawuu.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gfmqeqtdh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpukojgsp.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gwhimcpbn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gxfvyghxq.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gigbbzmmq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeqhxsth.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/ggngwhfpq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyqssozb.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdafrmmlk.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gskanouvr.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gvyxaukqx.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkzlbctd.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gerjkgjew.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvttmckzr.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grsmmxjcl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gnwfulekl.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gorvramcp.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhsfzubp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gqmaxapml.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdmawadmd.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqmcxlml.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnqsmpis.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gmpjlzsfy.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gehamvmzt.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjmpldrf.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfowtejwu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuznkvtv.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gdjsdyzxr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmelotuw.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gtxhxxdya.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgjaqghy.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrdnhnry.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/giqwkmvys.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gvegjkjhy.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gouonbccx.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhaqolyi.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkvyqwqk.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gxltgwemo.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gdmysatky.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gucegdxdo.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gfpxrbwcq.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsnwfmud.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmkfwwwv.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/grosfvkem.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gittfgowy.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gnwibmbem.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gqqbndjna.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghefgrhvg.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gbzkwymkg.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/glourtinx.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gogdvjjrb.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdnspirx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gjydftytb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmqmvlqf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvvdoqum.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gyfetxxbq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/govoiuunt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweabgkym.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfhgohsv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdygnorb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpotkfqxj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrjpgfhx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyqmrjly.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gqrukbatc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjvxqvur.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaazppfg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gazryfqfp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gefahdtsg.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/ggdnpamzj.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvzjwsgh.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gehaibagi.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrerpauo.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuzzbaeo.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhonofv.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbewqvnp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojnquwdr.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczwciajs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoznwihz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbneiehkb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gozustawp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/guahapsnh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gmmvjydln.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gxnlzzggo.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqfacqef.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnncblbu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlbycdwu.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gxhytlphl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geekheuhy.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/ghdoqeitj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gidagpuah.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/glddfmoab.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqjchzyf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbfgpfyh.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gvxurzghn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gvfegthzv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gweelktyj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gmxptrogl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gpodtmcgz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzpxqqli.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmnbdrak.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpqxcwsx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtmzvvhj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/ghseruovm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gllitsaut.sHtML


<!-- 参考信息 -->