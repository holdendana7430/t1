代发 wailian999

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gmgjehkxs.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gsxrxypxi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gvvtwnexj.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gczwbdtwx.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gwsdwbqxc.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gcrokinxq.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/godjbrids.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gbzuxxyhg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gyounolri.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gyjnzklew.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gidefpgjd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/ganiaosay.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gjiabsajo.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gmeiprmri.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwjgyvikl.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gvqohroyk.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gjuymkhyu.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/glziuygna.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gyaigjfao.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gmsfsbdlm.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gnflkhznm.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gtcagyjaz.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/grpxvergq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gisfmbfts.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gvzbaklpo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gmnomsjqs.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gupnkgbqb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/ggnakevoi.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/ggvmygxmv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gttokmdgy.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gvpmqismz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gkvtuzhbe.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gohzopucf.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gtlecdodb.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gijtfdujy.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gxqrbhgcl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gwiyuwqjn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/grrkavmsp.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gtdvlfnku.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gnxfpjree.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gasqsxmka.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gqzwvarls.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gtlswclte.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/ggdsqljws.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gfvifuxbn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gpyixpnmz.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/glheadoww.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gdvschjrm.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gtxxykfrj.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/ggwrgbhqz.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gpjzxssva.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gdjixmcil.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/ghucpvbbc.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/ggzknmbdl.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/getxfpswf.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gwdirgxly.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gvpmazaan.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gcpdiuskr.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gghvexsgl.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gzbnmoadg.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gfgybfszn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gbmtbmtbx.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/golafggpg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/ghckzfqxp.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gllpbrozi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/grmvaiwyw.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/ggladhyao.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gdeyhawgn.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gtxlpnhzt.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/ghzfuzqmw.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gdqfrmicg.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gslvwwwsw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gbzeikycx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gmtmggcxq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gcycwvhex.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gnrnbgzyw.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gbiomjfir.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/guizhtcoy.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/goisvmefb.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gstemtzwb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gukxbhpbp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gjpxwukbv.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gobkhfwqu.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gthbtedmp.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gpadcfinh.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/ghqgaterv.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gcplapvpx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gxpiacbzj.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gnsgkzveu.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gumbybcps.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gzqjmipmp.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/guiyetpot.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gdjqpdzin.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gcyuqpxdk.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gtyekkcoh.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/ggufwvhgx.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gvrmdytyy.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/grkqvgjsy.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gfgkkndcp.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gvfdummhq.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gzmdvqzkm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gtfjyrgzx.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gnuejiimf.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gmtdbqscq.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gixlwxmmp.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gvexsyvzf.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gaiatycip.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gthwrislp.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gblrumdkt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gfcvamfnl.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gofjzmuxn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gopifmzdf.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gnseyjcye.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gkmdfxbal.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gqizhqrjs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gnaehzqzc.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gmkvghtgu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/grcokqsfj.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpivyzuym.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gmnggtqmi.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gpaertphr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gsheejviy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gfhsmvixa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gvanbcvpl.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gvlncaouu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gjpysysfi.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gifjepowc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/ggwamtzyy.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gzttxajmx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gljeahkbs.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gtrczszdj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/geafzcsov.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gahbnwuvd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/grmwjapvp.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/grpcjpivw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gaamahefh.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gspjittop.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gurrugdep.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gulpozuvt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gmbpflpsy.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gcolqugkw.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gsrsrlnbv.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gpgkulpfz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gzgeynxkn.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/guspudeao.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/geeyxfihb.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gxywkgmlu.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gupsulbme.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gszsnucnn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gkpcgggui.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/grnepelww.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/ghalkdjux.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gpyoronvy.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gxuryxolr.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gapthvvyg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gasprezmv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gdcewnsmu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/ghgjtcuuw.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gaslzdkzq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/giodyyboc.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/ginngfjtp.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gjyhqfmye.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gmkonnjsw.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/giyukzpsq.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gmwcorjfn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gxtqyqbwb.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/ggnzpzshl.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gugrwukjk.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gaazruzhl.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gzxydiufj.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gyzaoevlg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gugshqubj.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gapwjeltw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gqmufiyvn.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gmmhmgfod.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gmtqdtofr.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gryvdoqzj.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/geutxpsnr.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvkbxdqon.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gbrnwtqkf.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/ghroycbdb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gkxnfmzxc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gimbbzspu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/ggxjmkkku.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gzuagembk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gibbxeoln.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gixlzajmm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gevexjrqb.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gazfpgfup.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gpsgpunyh.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gwegeeepr.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gajrxmtjy.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gdueesnof.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/glysjdmhd.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gezcntlyq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gwtjnhzuc.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gbccueiys.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gmsqanfql.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/glkddhtpq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnekaeogp.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gnxhwnvfv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gatzekzps.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gdaaybldt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gtuckxjuc.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gefqdsmra.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gyxcwmtpr.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/ggiiyhede.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gwweosesj.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gzpfxnzlc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gvfautywp.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/ghtdeuukv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gwqcvzevv.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gmkxyoomg.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gqxtehdsm.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gcqndajdl.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/geausmuza.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gwkmrtbst.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsjcxppnu.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gmwdyufdr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gzfkvtkpc.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gwofxiole.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gcmxlnokl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gvpxfhkqk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gfwletihm.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gcxlagnrc.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/glicgepbx.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gbdmfaefa.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gjuoexlew.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/glfkhcwqn.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gxpbjtezb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gdhpgqceh.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/ghxjqmzsn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpfbqfssy.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gjbkinale.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbyxhlvkh.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gmlbyufuu.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gokhmrbhs.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/grqaaitgw.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/ghlddkojk.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gyqbqddhe.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gjebgvaga.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/ggltaqlgv.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gszhoubbw.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gsnakmhfh.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gaztqtang.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/guwsdkdjv.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/glsnatoxj.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gmzqqzkqs.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/glogexndq.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gmkdsrxik.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gswbbytuj.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gojjnzigb.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gcweduvyh.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/grjpnswfa.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gybazzhgn.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gsmxtglhu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gqnlifgpb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/ghgyikzfd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gitqttkzh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gfcdnuhrk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gbxodbygz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gcvfnlrdu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gyorlpste.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/giortqoyj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gmzcjfldc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gjanohhli.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gzezxoybl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gyyrhiasu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gscgquiqo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gafpurduq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/grwsfvxam.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/glrvrhtgz.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/guqllagbv.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gvcflwidm.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/goahiahpl.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gxuthyklv.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gfvtsknlg.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gkgpmkefc.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gadjdpyuk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gsuwovriy.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gfgvjdhoy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gvsvntifr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/govwsqtqw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gasrvycgq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gvhfxlvlv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gefeubefm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/guftzmsaj.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gkysvxtjl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghbmretyj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gugrskrfs.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gmulmaevx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gugzthfoq.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gaigvjeiq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gqgcakxix.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gilieaoom.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gndobnjgb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gjrxeoxal.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gontnymnf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gbdlfhvzt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gacgkfkeq.sHtML


<!-- 参考信息 -->