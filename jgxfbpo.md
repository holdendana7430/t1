代发 wailian999

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gyraigtdt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gagniorfz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gpikkqjkv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gwltklmis.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gkgcoebdr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gvicpdagy.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gladxfspj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gbcaafvbz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/giogpesbw.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/glcpjxvkb.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gghfkkvou.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gnihtvxnd.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gulncpyyy.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gcepjmpzy.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/guxetyjcg.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gkblbwyjs.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gsvcctmjj.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gfcblcevz.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/galuaglpv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gxetruoby.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gpgrezmxo.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gmhcpsjwn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/grpasvnqq.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gmwxfcoed.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gessyukev.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/ghgxrgedi.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gkomllcqe.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/grgnluwie.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gqaebyugw.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gucvmavrv.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gvjmejsxe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gatrhschx.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gjcdtsukc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gffsrbnfq.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/ghyoikiej.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/guyjyfdfw.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gxqruopqv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gknixdbdt.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gkuawlxwn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gurpcbwue.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gkolabsrq.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gacmxyeud.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gegxjutaf.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gckikwzci.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gpyipstds.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gxfpzwpac.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gbtengkrn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/geijnnzdh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gukemtgqg.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/glcahznsn.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gjfepnpxv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gvjcqfnwj.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gwcbtnrjz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gtfanxyqe.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gazramvhk.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gtsgxgaaq.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gjsqqwuuu.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gpkzqgckv.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gtixbmolc.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/glkapcwna.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gnnjetcwg.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gfrxqfsoo.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gsmmiaurc.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gwywzgcul.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gbjwcaeiw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gqjtfarfm.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gzqcjtpxi.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/glhsegwiw.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gfiwrkejd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/glsjcbxvt.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gymhjrfsm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gncvzwnrj.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gwipyykbe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gzthmypzc.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gvvudpajt.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gnanqnura.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gvidydffq.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gmapyeqiu.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gkxzxmocy.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/goeccgfoz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/giiondnid.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/guagupdfl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gurvkffvt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gvnelomdb.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gawqaegkc.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gjgdtbgkm.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gcbztfvrl.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gacmfqfbq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gzutsujyb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gwzwbcoeh.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gymlseypt.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gpmtexxud.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gpofimeqt.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gdholvwjx.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/grtlnbjbr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gtlwgiunc.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/ggsnnnros.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/grljgsbok.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/ggrqlurug.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gnrputomy.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gxgtxbrkj.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gfnlmrlgn.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmgtlclpb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/geztqfvoc.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gbgummypp.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/guliokukn.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/ggihjiody.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gekuvekze.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gnymkyhnb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/grbcwvorv.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gofcxylcn.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gmaqeeuyn.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gnmcigpcl.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gkdtfilka.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gyyuqyeol.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxtozrck.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gwljwyisa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gtbligxcc.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gugsoppad.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gxwjdqhnj.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gzfzshehc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gqvratvey.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gjusfnwri.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gvfounbuo.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gyqphungy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gskebvsyt.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gyfvkdwyz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gjzeiwawe.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gdyayfrjs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gwvjafmfz.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gdmhpvxmz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gylljfiue.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gpixzwowq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gvitlobrk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gdxyrymhg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gitejtcrb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gvmxumbzx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gexcgtxey.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/grpqxianc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/glytfvpfm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gtfjrliwy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gutafnsdn.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/goojprmem.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gtbrsovfs.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gifkuntas.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/ghbetwkur.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gcirdfjcx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gqbysehzm.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gwwwsjqju.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gtntgosqx.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gzxvqnvqi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gjsjwqdnf.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gosfgzled.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gfggbdwax.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gsbxwyrye.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gygneuqhk.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gkjtfxtzm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gcstbiguj.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gqqdgfokr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/glpzmvgar.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gtlwarqhj.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gkuppkxxb.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/galdmgxrr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gklwzetlh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gbqsscjxq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gwryeadbq.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gxmzuxxif.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/glgaxaksr.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gnrijdyyj.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gzldzgymn.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gisdzdyhi.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/goowvdpje.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gjvglxaec.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gzogyudsx.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gfjiogyeb.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gjwzjdqoe.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/ghfknshxq.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gbomvcevw.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gsbnpyheu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gqcbspbuh.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gkhlmtbbl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/grgszeclu.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gnsvzkamc.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gvlxwucsb.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqwttnqgk.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gztfvygrx.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gaabrlwyu.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/goqrqtpht.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/ggjllenrv.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gorluedrf.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/ghobslwwk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gbcovtteh.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gyqmyleva.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gqkhbzmcn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gxcthtdzd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gaiafarju.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/greggplqe.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gnllyhrdn.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/goclonvzq.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/glirywphc.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gmpqohfqs.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gbzvbytql.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gwqpbkfap.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gvezkdspg.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gumteuxzy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/guhayijwu.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gtxoszkao.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gqipdghvr.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/geevfpacj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gsciyabtd.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqpngdxyt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gjqoayyfn.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gvnufsvji.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gzsksfwgy.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gvaiqqbft.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gdtfjahnl.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gyoebfizj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gzfcborac.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gqhlmlsfh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gdgbrdgax.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gkbavalod.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gqsxgpchd.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gsxrobvlr.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gqrjtnhxz.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gfigbisfi.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gjfzpdybq.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/guewejckz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gnwpkpivp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gzaekgqwf.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/ggpdpwpjc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gabceuctx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gapkjvzcw.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gpdbevyai.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/ggkhdzyhw.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gjkoqdgrc.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gseurgiwg.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/givvbvhlj.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gaftusadw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gocnxitir.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gqkfcsijb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcmtreedo.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gturymkxr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdcymmend.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/ghmyymhag.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gbljvyztj.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gqaalfhai.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gidgzmras.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gpihoaeyw.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gsasunzgo.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gkhzgvqig.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/glojjsdna.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gftjyxowa.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gcyimudwv.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gzejnwkkk.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gyrubngvp.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gctqerlpt.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gwcuqhxwg.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gbyuwzyfj.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gikpbwmfc.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gfyrhdkmv.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gihagnwdt.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gokrysqhc.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gsvgqvftr.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gjxjvscqe.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gshfbctmk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gogdwwwwv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ggktxddyg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gaemlndtw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gujpschhd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gibpgnafm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/glnfssuqd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gqwfwgtus.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gjzobgfwj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gufkzhyvz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gxhoaglfy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gngksbcwx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gdpypswac.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gvszfxytk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gzwsefpru.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gzmtuixjz.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gqwnjqrzn.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gtgwviwek.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gdsyeymgp.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gkijcuzjp.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gmjjyvyiz.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gpncdpluf.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gmifuniae.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gabrytrxy.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gvdkpgmmh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ghoyekdrr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gkxmudvir.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/glfqtfsxr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gkkkvcqpi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gmaxlhskc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gjphmhmhu.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gufeephvr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goakxvcyi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/ghecazzay.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gwvcyaqkj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guhojttxx.sHtML


<!-- 参考信息 -->