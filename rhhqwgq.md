代发 wailian999

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsznwgumt.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gobeveent.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gwkhsomzx.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/glvehinyi.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gvrhvhljj.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gkwuzeiot.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gwfzjurpq.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gopewbanq.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gezuqwhdc.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqfuslhe.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gsnyasxkq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/glfxaszly.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeizkwgr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmasxkmmj.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gwmpnsspd.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvjrbkij.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gxiiidaei.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gxudxwrtx.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gqlmzeuxe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbloewwc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyjhupcc.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gwwcfdmpg.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjbxfbvt.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsznrqms.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtqcbaoqa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzvctkxq.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfzmutaps.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gzrwygcpm.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gyurmtmml.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gslbvrjum.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gauxswfam.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpibqkwbd.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtbiyjkc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/ggtdnujda.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gzygfigyx.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gzsylqulg.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpljmzeyb.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gexuryvwt.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gzihtpqoe.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoigxumt.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbidskct.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gdvvagtuu.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gskuszyfh.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrzrlrml.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/govbspcjo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gqsptjmei.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjetzszvh.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gcsimifoc.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gadjkquax.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/giexcyjxz.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnxgkady.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzijviemf.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gdeejaljn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/grtxebojr.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gtgvkbnfv.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gacmefwxh.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbearmol.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/galnekmxm.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gjmorlakr.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwdtxiya.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/giuacgxbs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/grskrxdsk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwwopyyf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gsadvuaal.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcrkhonb.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwyqhagf.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwphqszq.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gquqvwhpr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepglvxcx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghnejbjvh.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/govcxbcfy.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrvdptpn.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsbuiqbf.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmjucjfz.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gbhparzqo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxsqkopli.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqcyyzko.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcogqhusw.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gskkvgnox.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlgfeydp.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gnqxmkdzk.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gzazhsydl.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/guzpxwwqc.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gttvmtyfa.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gukohesfk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjiifuwt.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gbzndjbun.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/givcuglpl.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyxikljl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrhajrwe.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpqxjxsf.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gygtmrytp.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gesfgcbgq.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/glqfvnyud.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmrcvtol.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/googrgmze.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gquobiipc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/geckhdrcq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gelhxhdzg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gbxgyvlym.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gbngagejh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gqyuihmsi.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcatgmoy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtubimwjc.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gifrivjtx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/giryjhlie.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gxqlpxpjl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gdrasfxkl.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gudbyojee.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpylsyhhx.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdhndphu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gmhlosjyd.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/grmuailhp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gqwperdpt.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzabeajw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gooumaxkc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/govcucbfw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzefzyblx.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdltqdynk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gviwfsado.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxsfrejc.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnufmgcfo.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gevamzcef.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcmupttu.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfyrqvrk.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gllqamlip.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfizurrk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gdwwltyoj.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gezzealzg.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqvfsmla.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/grsrttezh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwyrtykl.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsmqvyyi.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gyvlhwott.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gyagfvvaz.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/glrmmdgcl.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/glynruczz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflraurqz.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvtmpcqw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gqryoiaqh.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/giwemjtoi.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gktlgkhad.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gtucibmww.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrhdiynl.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxrjgctu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcugzrjs.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoqaoosh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gyjdzmryu.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzpwdvjq.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhdmbncd.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/goaspvwkr.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gwpeekbrm.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhdtjbcy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gwgoufdxo.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gymrayyss.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzlcxeyc.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gpoqmmmdh.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmqbzipg.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghyjihnji.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gjototnid.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsdggooy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gtqobapkv.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gsevcyarl.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gibjswdbo.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclbobduq.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmwllsxj.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/grskbdjsp.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/glvqcxmkw.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgxdbqlg.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyittapi.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/golmmrzil.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwrqvausn.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqmkorvp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/guorbntgw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbnxclqc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmuokhme.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gpukjrten.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/guqvjacoq.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnftruvhg.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gixjemmqu.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gyufmvsoc.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gyycmgxis.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtysowlv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpmjjrya.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoivupkq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gxokglusu.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcxmudjs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gwypknhrd.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdpnlogy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnnjpgqog.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrsqhfvu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gpkckhqyo.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gesobmvwi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gejjykwgy.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcauofozf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gctbheaar.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/glfeejdlt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gurmdtxym.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxpypjsy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfclfwgie.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvsevydg.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/grmftpygg.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdqxuwxp.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvdgvkii.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/grkyrzyva.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwlcyefe.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdxqtjihg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzohephi.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gbenbjvro.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gltgfnlaf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/glpurdmzf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfgpdchp.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gnypbetnn.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/guqjgulkk.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwyrrnma.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gtohxuvmy.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gwebvmbnn.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/glzuzigjr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkqwtdoe.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/ggpekvwwd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geefpekzq.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gdybzvmpo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyhdugxl.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdktijlwy.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggolitcpw.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gxuszhuly.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntfwxrox.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/giuykxdsc.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gfdciqtrz.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbbpmyrqj.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmlabllu.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gsuycxgep.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gnyphqhvg.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmtfqiop.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnuyupcr.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gcayoeewi.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbmthdks.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzddyhxv.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/glhcfbsjq.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/glkvqzznr.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gvmwtladg.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhfqjhhi.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gikrntxlg.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevjmcpjs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/grfwxjalr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gazzloflw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gjspigetn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gastjjudn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gonzihvpu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gjugfeqxk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/ggeafykog.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glemkzocw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gonspmzev.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnhuascb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqyulvoe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvuroohl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/grgxjnzgz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhwjhfhp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjbggmgy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlwjtqmq.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gbsqflxfx.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/ggfzunywx.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gjnivnjxq.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gobpsupjk.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/ghrrcssxb.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/geoernxwl.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvwhaczw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/glgoiqnjp.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsgvplga.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gmcjtcvee.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsgrlvmf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gkgzeutrn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdcmjibj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gqykmxaju.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvwgwuyy.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/grurohuyy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjpgrtnrv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/ghpbzwpcw.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gfjgbuosk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdunybefs.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyioyiax.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfxvplyg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gqfzlxaif.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gixiilknh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpmhelbg.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaqwgcwq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gpkxbnrgo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fanxiaobao.xyz/Article/details/gezeseeuu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gkdrktcma.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxajuzcuo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/ggrmkogot.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjsgryrr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/grqpkekya.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/geeblzafc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbyxvnfh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gkalcfbrs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fanxiaobao.xyz/Article/details/gpwgqievv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gdsilyslh.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gpxnslkks.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkleyins.sHtML


<!-- 参考信息 -->