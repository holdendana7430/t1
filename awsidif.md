代发 wailian999

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gvlyjonii.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwobbwduj.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/geysqslpf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxveqswtx.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/grisljzzz.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gjvbkmifu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhrzedzr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gdvwceinp.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzfjvoxj.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmjsexvy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grkdwmiru.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxnuhbwv.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gduuoptru.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqfvdrxk.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcsgtixe.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjqnlcin.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/goxfebgsr.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzoirufb.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gzofvoysw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gzfukpgjj.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gunjcjjdd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/goweyfirt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnsycxqi.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gwdyknrra.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaevueqb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhcaprts.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/grdiybylr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxajbqlm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrnygsai.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gizeddqql.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotkkmqgs.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/guwwtocgf.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggefpkqgf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/guiticcpl.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvezhksh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gimihcrrq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gszdnaqpu.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gakyrydjo.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gzcouehgs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlujjpfo.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gztgrwhcu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gmjcniuge.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gvnyxnweg.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmqqcfam.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/geatghszb.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gcdgmrssa.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gdmvgrpbx.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqocrpnc.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gecjuaqhv.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/godovtayh.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ggkzgeoey.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gcnwqrncy.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gubsfnrws.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gednrkxzt.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtttegbgj.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiygyeeg.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/ggfutgzlf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggafcwmbg.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gwatrndki.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gokiypfum.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gmdsmrgac.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gzdszhtpp.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/guenznmjk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpgzwcnx.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gacemxfgt.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzmpsrrf.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiskcebu.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gidrxpzlx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/ggybsoruf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmwbxddw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvchbacb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gvjnzsagz.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gobplairq.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gjlqtsndj.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyidmxor.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/govugkmut.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzkumdyi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/guhwtnove.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gvwcpkgzk.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/ghqfiagts.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gwsndszcb.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gwmgefdyt.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnkiwubl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzbbhmia.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gmuprxvxf.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gboewnezh.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/glepaxtfw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkmnnizd.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gmpplmfen.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgduemdq.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghpatffmx.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuueoyxf.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhbbbsdb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaettcej.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpejkuqop.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhnsqsts.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gxyqlnabr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gvpagegpk.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedffsbwz.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsfybeqms.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gtzqvwhng.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkimzoppt.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gjpstjvbo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsebpvfc.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glhrctsmg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrvygfwy.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsgzddey.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/guzcsaaex.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gcvzintkf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gauzonsij.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiehtaos.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmpapjsq.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/givqspwbn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxtscwlk.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuuzcibj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmntbdlf.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gtspjlyxy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/geadhdmwh.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gguhujfda.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzymwmfy.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpjunekl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauxnkbvn.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gcagenvko.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/grngioesy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzkenmsr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbcgdqcx.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaruonbs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuolkcpt.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gocgclomp.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gzdqwihlw.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghgwklgjp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/guhbezocg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gvheurqwa.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/ghrlvlcsj.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcfynramq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gsdqsjdjo.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjilztex.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujmofhmt.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfmbedl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gtvrrhoft.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofpsypkk.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gytemiuyc.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gxnmvsubw.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/guqxqrdpw.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gywjaknwt.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gecvrfjpj.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/grsmvomsq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gnphhosix.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfztfirda.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gwkzbrhkc.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/ghnhebery.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grcrvlhdy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmykryjsr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gozssbdsu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgrcetdl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gjpzdxlvo.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqmlimho.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giosorpxx.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/glnsdgwwh.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpvqclsa.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/ghbmmvkny.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwllcfsoy.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gqyxahogq.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmybyxgc.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gsufxcdaz.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxogajwmy.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkweopfrm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gillkhdkz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gtkhzaaaw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzaqyrez.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gryeglvau.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwskfjvo.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gpxujenjj.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhqnfnrn.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkkdxdeyd.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gfgbmieur.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/glmaihvbo.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gictvmkwh.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/goqxzfhdl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gelxevaub.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgfvixek.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gfgvuqbly.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gimmeboiq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gkdqeshjh.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiscbjya.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvyjfslg.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gcbylpdhq.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gpkdtktbp.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/giheoetng.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gihkxvkga.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gcupnyubd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gnfjjvolp.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gmkqllbjt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gqxmgsotu.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgtoymtx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/genlsdfrh.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gnrsurjzs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gswoezyjw.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjvmirbq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gnngjnfeu.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gxqtnhmvw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlivwlwi.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gqipvwzyu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/guztmubgy.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnymxkjfo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvyojjdz.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gvyzbbxsb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/grkocbree.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptcivrxw.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gkfgyjamk.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnanuubu.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gyxplmbnb.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizncbwxj.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtyrixom.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/glkzzwotf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gdrhrxwcn.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gvluqrjlc.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gqzugwgtv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gfswllhuq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjcncxlw.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldkjitrg.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gvakggqto.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gjuymmieg.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gimwjzkgy.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gfuvjldvf.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gfqjkgtjj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gqxmatbci.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlhuglhf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghfncatfn.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gpmnjlwsh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjksvuurg.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzemjwmif.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gxehqzsqi.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gmltkksmf.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbykiwjrl.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzgucnjg.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gpoqiswpm.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gmxceckld.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gwqtsmiwm.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/ggphvbiya.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzqacbfz.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/glufchenz.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/glypnlwtb.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqhumizl.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkvlyowp.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gryzlgmiv.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gakvdtbwl.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gxymrkpjw.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gamfhkwnw.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrsybdji.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gceerfkgz.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsblunyg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gmugeoosc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpatlwajd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklxvxxbx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexgputgv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gabqpyqaa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gojffndrb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gkkcormkl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkodzhfg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gpuczgosk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/grzbldgea.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoycfvls.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/glyaiitya.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwehwwpac.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhgiumnr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpmfwmqu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/glpwaevow.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gajnuvdvp.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqttdstj.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gsizjsohl.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gpiksbthm.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/giblmrzjh.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlrtpcut.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjyoxioq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gtryjbrml.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gkioqjmox.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gwiqotbtg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewkeqive.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gemhtwviz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpwiijnf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzpqdvii.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gwnzildjd.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpivgmned.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpbjelwp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdunrafvd.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gvgkwdlbs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhtifzyp.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucpmnrwx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/ggpoepjmp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbfhvbsk.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrmmtdmm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gzlhxagax.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gzadobirv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/ghvbuttgh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gtvqosccq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gwaglfpzt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/giwsgvhyh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrwfagur.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthksuhmx.sHtML


<!-- 参考信息 -->