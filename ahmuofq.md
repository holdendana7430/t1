代发 wailian999

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/givsvqyog.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpksluxaw.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gekiflqsd.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gdqayhcra.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gxnvuedpa.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gfvjopksd.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpicvjba.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuoljmqo.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gehhcdqtm.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/geiochltg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gdardsuau.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlhvklje.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxsdqprt.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giblklzei.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gzsrpmmio.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/grawtpffd.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gqehkqonv.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjmprfni.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gbmfwvhqt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndouapwk.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gmbrhnkab.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gpeoquzms.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gaigsozzy.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gojlvlbaa.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gevvfxlia.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/grrndqqwk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gplryuvmx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gbloepets.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gexeydabc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnebmaory.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqrkciws.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/grugggllj.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfwkldju.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/guhxlythf.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gagobuahw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/giogjtyiy.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gwehxgpkj.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gcmoopqwv.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwbndvqw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfszdkdy.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gdposlwtt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/guvefjfsa.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqocahya.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkohqbppa.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gceyrlexi.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gjrauyxgg.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbfuskct.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gtxuxunfu.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggewgvnru.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/ghtflohsr.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gpmhqeeuy.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtkhumyz.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhxyegyx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzynnntdn.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/glmatdqnt.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gywhvbrvd.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/ghkaiggyf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gzdnskhml.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gzezbsgfl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbczmwmvn.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gpymarjef.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnmemfzt.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/ggozpfmgg.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/grejdosla.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gvptppppb.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gjyoedgfn.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/guidbacyw.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gwrltffro.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnkbvlfs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrmuiukg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gibdqcedo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmfkilzh.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gevmeurry.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjosvcjy.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwtjqjpq.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/grmpeltqn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gujshmffh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyyujxry.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpwilfoc.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gaszfmcxs.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlkdrgvo.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/guhognmev.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/giyddlkgp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqgrwole.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnbwylpm.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/glodxfujq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/ghvqoueqs.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjwwjveyt.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakdpoiqa.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/glwalotfn.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/garmyyoay.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gxeriknon.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptegphyi.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/glxpqwjjl.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gmiweiayn.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfenajbc.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpfsafqv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkddqwgmf.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylrkxver.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gsmgswxjw.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqsvquln.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/geseqvhfn.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/glzjdxkvk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbcexlly.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggycjjlyg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmoqrsgh.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gsdngjorg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gxlgptevm.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gabyiipor.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gvqyapaov.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstwacuqo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gbfbukpsm.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/geexatmgf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszpxalxn.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gksqhvolq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gadvprxsk.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/giqrdsrhh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvkyrotef.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjzrprjo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/goryaitkc.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdqrobok.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gftobbaqk.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxaxgtuc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdvviryx.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gbujjdqyb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuegekfl.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrqpfhyi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gcedeuyil.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjvxnifs.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnqkazga.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/guxroqgmm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiufvqwr.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gnozwjigd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gagprlcdu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfzmjdod.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgrasdwx.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmuvmgfo.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/guifeycon.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gitpfrmzo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrnnqoea.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/grvhzjlxs.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvsadsdi.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbrnthhh.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/grvktzmyr.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gizxskuqs.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gluioxgdj.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvasapdb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gpqyzxonq.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbysgnnz.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/geufocjmb.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gukeoznmm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gykpxhzyn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvchsfdnk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjirjlkt.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuuusefw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrnsualy.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/guldsxoih.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfbprnyo.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gifikzcse.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkusigpi.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghspieagk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gjwzilhnq.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gmscrvmkx.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhkevrqd.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/ggjhrwzhk.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvinfjfug.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gncgzjjgz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdglzohb.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsnqcqka.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gldkzesni.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gorflmtqz.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsftdhxbh.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsoioegi.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gqovesfoj.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaqucvan.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/geaqxoapl.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gxavriwpl.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/glpfdjaxy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuhinqoy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtofywnen.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggexvnbib.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/guzjefsbj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbhtzrli.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gpmjowfak.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gspbppyze.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqdgsper.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gggsbqiwh.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwhlbujq.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gehfqhspa.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjinjxqvc.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gbocfxjaq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdwqaplb.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gcehecrgc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gswsbkkfe.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/guiyabnxg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/goeeoxlgc.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/guyfmrvbc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gfihxqist.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxfcjiln.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gyocdojnd.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/glllnakxc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gmjbmttjs.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbxawkqt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/goifaknql.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnbjglay.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gorjecjdp.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwikezwwl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnaxvxww.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcydbfdo.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gvmbfqewv.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gmgbmcvnb.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggazermcg.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gytztcrxy.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/godijzesm.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdfacmddz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/giooiohop.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/goanfoigj.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrejlhkv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxqblbeg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpqziwgn.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gciqyxnwz.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gvzaztzdf.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/ghggnajdv.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/guldpczkr.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/goyrxrrzf.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gxbeyehvi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjybwcdm.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/giysiuxrg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotimvvcl.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gbowgufnq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcyglteg.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgtgwucm.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggniratkc.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqkhefsu.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gzkejqkys.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gbtxmdjrl.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeipudbb.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlfjqukz.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gzavhersw.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjytlfec.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/geanyvqyr.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbvoxiko.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/ghaxtyttf.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gbjlsyuqd.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/giiejqery.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gceovytzf.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhjbadrj.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gdrziaqqs.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gckybinvy.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gxcrexkia.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gnwevxbiq.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gtftwlrza.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbyzojy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gpwxyalam.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfveszaor.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gumircglt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gsxyhptpf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gxderzfun.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldkntvng.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjmlnnme.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgggkjwy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gryawpfye.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdespxbw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeqlttbp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gajdbbmox.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbfkqott.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gxoxelbwn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gekvbgagk.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gpxvbsiyv.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gjzvzkwbw.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gttsepbhv.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gekpovnel.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gvxmbjisr.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gokiogtba.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpgiladi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwldgvgg.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gkdlblixh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gqinxcoux.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gqnzjveui.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gnwmfyfri.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzilckqzl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmghmywb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcogvpjs.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnushlkd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gunnmfssu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxuwndaw.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gizixjqia.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggskleihx.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gzfqdxtyf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/giszkohtj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gramdyeop.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdvohfqi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmighebe.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gngpvsvwd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyntkhou.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gaqaugowv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdyedssx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmfsappy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/gwbuwiaan.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyajhtwj.sHtML


<!-- 参考信息 -->