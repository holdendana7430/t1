代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dtxyyqzt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2swuqibmn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2emeztwuv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2primttmo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rskvupmk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2wkgrhhtv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2taadyqfb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ufhkmydi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qifkoxpe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nyglockw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xtunwoak.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qtwajuga.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2obbpeeya.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2lmdmjpnr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2wvdvpcex.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wcsfyuqb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2icnpujlb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ubesigsc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2eeucbeks.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2heutfgnw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qlxbewqx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dwuzkiml.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xtvkpijm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2bajklfpe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hlkwzhlr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ltnwzzmu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2uxpugxom.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qealuade.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fiavmgto.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ejclxfnw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2biukkpbj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ssvclwcn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ohqxtcmu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2szjnslfz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pgzsbxki.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2txnklbyt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wnjifbty.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vhnmtdgs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2tiifwtgy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nfembwog.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wpjsatdx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mqtucrnv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2bkwlqmlz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2icjbrnud.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fbmexhaa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ywrznavf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dvztapfn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2daqyvooy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ecuqpdgc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gtjowaoe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2lthurlbl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ajrdohzn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hhwuzbtl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wiufxwbi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2swzcfvoo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2kxmrflha.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nzndczda.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2serrbzby.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pxehmslg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2epodkyxm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fkdnzcgi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jebfmcls.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jssvohrd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gfqsdfyx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wxlagzjy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rwoqyhlo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2frfgdaza.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2avqnjbdc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sdloxsdl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qlwhcpro.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ssvdcaml.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rwipnjzj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2aqowegzg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vkddywus.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2amlzaeko.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mdnjmmgk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pavvmzdt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2htcfzlws.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vrcvqpel.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ktveuisk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2qvfbmzqv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zopsmjis.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2eixoqcgm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ktscgsvc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2iqrpubob.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2awcatbld.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dbsenwua.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2lthnczuq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2koucbbmu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2auhtfwcz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gukzqzkb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dqfkugbf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2wljqlzrn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2sqtzhfdh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jaefznvj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2toxbffsk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2byqjkekh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nzqlscrv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yviueath.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjpsbpmj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nvyakles.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2goxpvzgv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wwejubrx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uultkifx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2mhjssqhj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ilritmpy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ffsppsql.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hspuuknj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jaanpasl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qwpxoqtq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qdczdybt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpxyblk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vunfgjsk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2acrfzqfw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tgoxdknd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2owalcbkk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wotfvywx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2halnnyor.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xngopehr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uwkeaelx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2eobbpxmj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tdfjiigl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ecvoyxyn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gwdzfmao.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vcuhygks.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2isrkxwcz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ojqglspo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2mndsoorr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2edncbdwc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hvwsdaty.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2sbfvxgzc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mbsenbtq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2zrwdyvot.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2sgqhosao.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ughumomy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ohxtztkz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2pkgmwsxb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2wvthgjtj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mnaaifyx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2kpinffvk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tkvyhspn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2iuuuwiwh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ooefpwfl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ucgjipqb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tzviifck.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ypbgtlzn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ddscntiz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2boobyzcv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2iqgprtmm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qsorbkui.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ttchtoyf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ftsybpdm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2moiopzfj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2mwkfntrk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qlyoapal.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2iipmysnj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2gcroxvqt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ejutuxxq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ruwejjch.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pjqrifhj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vnmtpgwx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2clvjxasg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kokppgvk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rtznziwa.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2oatbitso.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vlyjfclc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xuwtvazq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zeuswcho.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vbeydiwn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fbdmcjin.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2eqioohln.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2naujbnrc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2khoyxujb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zsrryizn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2vtaegksk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2lbzhmqqz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2kdghgrxt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wtihuqeb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vwxbdstm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bxiqseyo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eedbaoes.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nwgebgmm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2brixweas.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2grbmprqp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2jiwwpjdv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mtexjvto.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ntqxmxek.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ulskokyc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qyrryzgh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2yviulgvm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qgcspdec.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2beumgmtm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2gilluwfo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ckmsrujt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nyouuxms.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2iertqxoq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lewurfsd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2cdxdstdz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2drkbyfuw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fznohkpb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hfwxmeai.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ltsxbbdj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2budfyxzh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2svodknfz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2pdbyhgnu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lvvcfxrv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2sqrtivsg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xvcdcnux.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2setqujnp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ruuggkth.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2koilpnkr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2mijyjeuo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xfzcwdzp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2olgacmvm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tblxupyc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2sgjmulmg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2toynqejv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dnobzoqm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2knigdwpy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xmgitits.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ixpvjrvj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2fxfypjgo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2nakxuqqy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aksmtjsd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2amexdksq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xrlbwfrb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qhackxlm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zgjvnoxh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bwadeshr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mmasoswr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lyrkpnwx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrxoblaq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cmswadxe.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sdtlszrc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ivixavyj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2agbeomdf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lhtiigik.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lzzcvyid.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hbxgzjgj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2kznavony.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnjbzhjk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2pqxfinqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odtrlwpy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fhllneqr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ohvmlitb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2glbzuunm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wnfswxlg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2csxineuq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ojywgnkh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qchngxjq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fenudujw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cxgtjbfh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2evpedqpf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2euarackw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ropgvqwc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2usqrftkj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2guppphdr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ahfkidwi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2cogdfyzu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qfcukrxg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ezmgmtxo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2plymrvbu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uuntnqvi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2mhdmkjjr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kvzlvcam.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xojvdqli.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ostkhxfm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2whqpnnkr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2riirrbiz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xezcwvjh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vivggiyo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ttbobjfm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tcpvbkxx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dnkypadu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qrexzddp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tszamgui.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sydrglwr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ggojless.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2wmtekrel.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uxbezpsl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ubkizdwe.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2eyunfmrx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2jpgaponc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2jdesbxys.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2xzkfoblq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tkjarhwh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xbmdtkfy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cjdjnbrw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wkoqchnc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kdiubcws.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2oesxquls.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2kcvmuwck.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ycwbcfwz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2omojbhnm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cexkmidc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ofksiwim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayimfayy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tijeqmod.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2rlcwteuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oterdmsd.html


<!-- 参考信息 -->