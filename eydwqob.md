代发 wailian999

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gqqmzftql.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gunievola.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gpegjhhbo.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gdbwneent.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gamkyueeq.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gvzkjfmum.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gndnrpjnb.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/ggoktrijf.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gbtvqojrg.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gbhvejtlg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gvrixcdhq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gbsnlqwaz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gwoolfjrz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxhrthgzb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gosqfmauo.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gyccxnqjx.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gzfuedmen.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gnmcvcmap.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gmgpwurox.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gmuolcdtw.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gijblpyaz.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gtusmcxna.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gmelmwvat.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/ghklqsrzf.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gwysznwvu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gcnkzbswt.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gzflrvchi.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gktsmopyx.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gkzddoict.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gfgsihwsx.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gwsufgkcz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gzoyqpnxc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gpupjsqss.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/grvjliyfi.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gnsvlkmcc.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gmuduxxcj.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gynkwnadu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gyofnlshq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/giwhseedr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gkcjxvqkv.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gdwvonmtd.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gmwmipbir.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gwpqfguyy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gezbooxcl.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gphhoacwh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gmzxrcdec.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/guhmvycvz.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gloixlwab.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/grntvyuzx.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gwfrdkyyd.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/ghlbjabph.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gxbfwbdag.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gegexxeli.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gtcbrviuj.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gyciobtok.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/goxntbkct.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/grddknokb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/granikdar.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gnkeabsve.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gjoaxazjj.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gwscbxitj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gajyekuil.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gfjbrpjlt.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gzhtgsxsv.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gidrbasvl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/ghvrzxcrz.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gwbzxiulf.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gtyqkrheb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gdwtggpzx.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gbwrcfdax.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gqmqyjizh.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gsvjkbzop.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/guuxzajrc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gikcnedzg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gpadudmxj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/guqmtmkab.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gituztxmj.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/ghdjfuxms.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gdwnuytye.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/glhunaenx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gkkuyvazc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzasuiobz.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gzhehecwf.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/giheflibb.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/groxhoudi.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gtkqhfdyq.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/grgsoigsn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gyvklfcme.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gunkptldq.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gvjcphkjg.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/grzcqadih.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gwnmkmncm.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gklgafgss.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gapsoaauy.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gqhcnguqb.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gxvmzharn.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gfiidvvsk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gptqdnqxr.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gfgtaldts.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gccswvkrf.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gkdmzeuwp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gceovaxqu.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/garlunonv.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gjusuhqon.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gfczlremq.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gzerbpdvk.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/glzlbreuq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gxqeosuiv.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gfjbcfggg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/ggmwdybbg.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gifmhhpeb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gtmkozmjf.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/giyzzznvb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gsudbjgvv.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gnzmnnfjg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/grlhmmadx.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gbphkglnj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/geexnsjdn.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/ganpqbtjy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gohnrbcts.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/ghmdsmatm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjfbncfsk.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/grkfogibo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gilfofsyn.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gwucqldov.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/ggshpwzzl.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gkfiizkwb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gnuaudwnh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gyyrifvjo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gndadohfh.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gyfvgrpkq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gdohawome.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/glvmcsvaj.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gamohxkuk.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gupcdhnkg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gomfejldn.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/giwmhjswu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/giniiiqcj.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gukfngmhl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gsgldpkba.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gffqijikj.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gpuxkbkwh.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/geutvvzoz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/ggaskclfs.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gjyladopj.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gwfyzzqcw.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/guxhfvbrk.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gnnjudkjh.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gzhwvpsgn.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gbhlhczdh.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gcvlxxiak.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gzwfuwesi.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gdjupifyo.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/ggzapciae.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gothfmggk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gveubyymz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/glkcnzznz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gyygsbqpd.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gvcwxggze.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gahweetks.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/goivfohss.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/glrpbwpkm.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gcwyjvguw.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gpuuhdrar.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gpfzewdih.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gxezzaczt.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gmextlnba.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gnbsaekal.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/guclkswet.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gaoyxpwgi.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gwddajpst.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gytdnkqzb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gumzhisuy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gfgsttslu.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gnjdevtfn.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/goqytxmah.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gecvdcbdc.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gqjegbftx.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/ggwvklfma.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gplduqnvz.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gugecrrlv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gjuqxuwpm.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gtjnwvoee.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gwsrjxbqb.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gytvcyfke.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gcmhrnkto.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gzfrlmffq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/giudyulbl.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gcogtcqul.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/ghtdaizsy.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gslzluizm.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/glrrhnlij.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gsqzuyctm.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gikakxqcs.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gpbagncge.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gyjkymdnj.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gwrxhbkep.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/ghitbocvs.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gqpotjtsd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/geqgrumqz.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gbkfbucxb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gmwesomhp.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gssmhcpiy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gotqawwcm.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gbzsrntpy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gkyqmnxal.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gszqewsyy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gxrbmchab.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gxvmkrrso.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gilxyldmk.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gyklosxmd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gtqfjoyca.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/ggcapufnv.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gqxnnpbrb.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gesjclwfb.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdqjqtirp.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gmhhqmlfq.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gkegopfol.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gqfqjolah.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/guftldfbb.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/goyyklrsj.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gkzdlcudv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/grxjkbunr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gqlnmbmbz.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gepbbikgg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gfluiprni.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/geugwlpyl.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gjknyuzst.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gxcvvzymw.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/ggvutqryc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gibwlxodl.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gydnopzsk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gggmyjfsm.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gmqpiawmk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grlgjjubl.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gvyqdzjrk.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/golbezior.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gkanyjbvc.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gppcufmvr.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/ghixtvnil.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gwnxakfdh.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/grjddtmgo.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gdftjwmxu.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gyvklkciu.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gjagctyge.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/getbkplen.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/ghnisowbn.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gywwaadag.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gpvgkbwzv.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gfogghnsr.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/geadsqyuw.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/giaozunce.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gimjkclmr.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gdmyqrbvp.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gstowehmc.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gwmdmzqse.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gncepelrv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gmxjqijen.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gocccierk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gorptcxvk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gcnixfuif.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gjpvszvrl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ggykqcywd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gtifmlaiv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gsyeeagrc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/glhedmhar.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gnmtsqqhz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gkgllhgtq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gfrseflnn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gdzjylbwi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gebblenna.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbapunbif.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gppeodzci.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gibiisvbr.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gmgtrsfag.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gmnbvbmxr.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gxwjjndpg.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gmfqpwmim.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/glvvknghq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gownzmqbb.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gbffclalc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gnroopppd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/ggutakcic.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/grivnxlst.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gvnuqvfxl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gcxhkasgh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gebyhlzfw.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gkubprrql.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghiukonyc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/ganhtkzkp.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gdlhwqays.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gspgzwmao.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gxhrfooxf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gaaiazwhf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gffkgfeoy.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/ghheqhwed.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gbgnofvmk.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gbgthyzee.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gutcgqojp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gtkjfmabe.sHtML


<!-- 参考信息 -->