代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjkcqfuo.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoyktjam.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtyukzta.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcammgaca.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gkrdwgfsf.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibtqkqkp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmxocadg.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gsuexmbbv.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmsxbcam.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gwcmenxzj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgnjokql.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjcjews.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gepnwzmuy.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/garjpeuqn.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/ggjgssqcc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgtdbkdl.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/glbnjumky.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gdlbyeiwe.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gqghgnogb.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmekwaxoy.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gaylraoja.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlmifpsx.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/glatkahoy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gaxyvwgsa.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjvrjeqp.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/goldkuowb.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/glahukfkd.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnetcjjs.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoqtpcpr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gntqoegrh.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gqdaqdiff.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/guarmdqss.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gxorqnasu.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxwjbzct.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gxkaakhdx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gazhfyjiu.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfthkqoq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjgfeejd.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gobtzruxn.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgqhxmwj.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gaujyhira.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gmbzxsnek.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkqcrwyp.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgktvfsr.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gmzbxousz.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gteyytsas.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfaiiulh.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gknbhoavt.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhfpeeyf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/geklkpwct.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gratnlxlz.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzejzrpcr.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyxgyusq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gepxjzcyr.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnibbuwi.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gydazzaee.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgyqbodn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzmznigk.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gkjdmzpby.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzqbxrqz.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlijztvn.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gcakgrnhk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtyllnnq.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gxjapzdpk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gljinoajk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgvlxcbl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gkudskxxj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdppvkccx.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzrxbneu.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gyswetkox.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbdsdzga.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/glofktcwu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwamwkvx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkzpgowas.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gjmszfduu.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gobfqvxik.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gahgkasqv.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbiqrjfg.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/goufcupqo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwrtgkqp.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdodnsmor.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/ggddlwrrn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gdrmxgmls.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjgmbnob.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/ggcluzawd.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsshsjcy.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdlobqiik.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdogrhcwq.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gkrsuilab.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gibsummnu.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/ghyzqlvtk.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gqfsrtcqa.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gywdliaua.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqguovqkg.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtvtkfui.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcfdfgwt.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfhixsvy.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwzvzlph.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqwgojtj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnxbqjkh.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklzqbkdm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gynhqtqtf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqfijugv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gbcunjgzd.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzzocchr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gueamkuti.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkdduwdh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gmikeujur.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/guftterpq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrwrtohy.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaivaudhb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/guqoziofd.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvrhzadl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmbdiqza.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gaxtezjwr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gddnsubvb.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gzeklrezk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/ggpwgprdf.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gmylqlmvo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbijrnaqc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdapgryz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvicogxe.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gnagdrogk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gjkklnitk.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gtjkozbnd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhyjgril.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzkaicvg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gevxedxmd.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/ggncakxna.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjyjawnc.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gziahdaap.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gtjneiykh.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzeubimg.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gndccvklw.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gubwrxpzw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnttffrl.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gecdvzgts.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcsedpme.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbgjvkfk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiskbgbx.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gapnapxom.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gwrknidjy.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gobtfavck.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrmsyfnv.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gzwjdjvfz.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/ggzhwmstl.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnytwhjl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsultwisk.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gsbgqeapq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/giklwkxyd.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gimqtdpht.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyokpfzzk.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gsctfjyoe.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gsjwqmdiz.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqhwznlh.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzfwuinn.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gzxhoobyi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjscfnhw.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gqaocqktn.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/glrhzmbhb.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gggdknxui.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gyhmhcixn.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/goambijrh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwnqtnrw.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyxyekab.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gainlgogn.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuntopgd.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxslqiuuv.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grokdnysl.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzboazfdm.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmknvtnsv.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfjvyqqs.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gkjgjnmkk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkniftpn.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gtetwnlpl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayxoqpjn.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkzocwhk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gbionwfuh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gszgwkiqm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/grcoiwfdh.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gepslfmdh.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gcvcfmjzc.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsomtfbe.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxexfnjig.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gudyiodcn.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gvwwyrtyf.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhddfutt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbixcjya.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gozhxgtwv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gttcbnspz.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxyaodpu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/ggfeglvyc.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gpyihkwvb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gfwxooaik.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gwrvpadie.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhdjkfve.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gerzezgjk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjrzilfr.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gthmabyyh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gtqvwwpsi.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxnnjibv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gxrdtdsag.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/grugcbkki.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/grmsrlwkd.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwgwhopn.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gyvyokbns.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gebanigrr.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/ggczikowz.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkidvmv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfipavvrm.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/glboulvup.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuszgdcd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gcassetpl.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdvzscqh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gwhonhkfk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcfajeou.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsqfllry.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/guyytqlnq.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjgsrwbr.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyuobpqo.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gitaltrlc.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/ggxqflpzp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlcawxhc.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/ggnwilcbh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdtgxffg.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnltmgemc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxmekyuhv.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpgkqiey.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkdcsfwe.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/givvynzlk.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/guiunkydk.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gqoyqstkt.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqxddhyf.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gfpobflkq.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyntzvoi.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/grgsqelkx.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gsibzhkhv.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzyxnkmb.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gyklmgpeu.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gqhbvukkx.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gvlemnzqp.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgzxtozi.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnnfmcwe.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/ghvqutxrc.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnlvtkkn.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gedpwmayu.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gjglqgbwm.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gpawfkuot.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmosutir.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwnzizko.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwktzgbwv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpdxfczj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqziejdv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gqrfryswm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giewimlbs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/ghfmcpskp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/ghamyclow.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gecokcgzu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnuayrog.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gqfmvsipr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/guhmfzwps.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckugxpcc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gacxlcsbx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gbujmsdup.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/grlahfqiq.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/ggxqmcijm.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gjbzaalsz.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/grycuvbed.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/goczfnjsa.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjztnegca.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeytmvgc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxolmjhgl.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlwfbuwt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcutgouw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gwrqptkrp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gwksbkyyd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/ggyjlmcha.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gdymgypvk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gqdghxhtg.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/goegutysa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giwnzaeyp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjnqzubl.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrlhusbp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquizltcw.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqdnslqt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gdpitdibp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbauboxv.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhdlvebr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/govlybwgx.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gyuolplkh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gupszrubq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/glhuorxgl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gfjllgeml.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtzcrsej.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gahwcrtyy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gmpqoegtq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmjycriz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gypqxqvef.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gqkpsnqlx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gqrpupght.sHtML


<!-- 参考信息 -->