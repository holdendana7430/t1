代发 wailian999

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvziptvrh.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gyvflpgcn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gjlxpibbg.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjedmaktj.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbodgkatr.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gljivgqye.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvbaawbh.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnegamzf.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumxkdbbl.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxflsbufo.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzviqtmq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyzfqwrt.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvswmzld.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/grqpghtfy.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gosowutky.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfggpbebz.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gskhkicgl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaxkryur.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvslnfau.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gjmbnfjfy.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gmyadydwf.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gnattopzp.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmprjzmqj.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkqvxfrx.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gloqnupof.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjglrtlt.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrsuojwc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gggmtjske.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaszhgzv.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwbzbdcd.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/goqczgmcp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gjrivfcrx.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjzntwoh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gahcpcodt.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gepgplzpk.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/glqdeahdl.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/glqwjvbhl.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkkpxlus.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/giaohcemj.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghywnrhch.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwnewioj.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gonxyidqn.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gfezgdjpa.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gmgfrcekv.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gedvevvyv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohdpvrzm.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtatcmkrg.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpsbcxvd.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gfhngwpnw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmpdcgph.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gchmotnsg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdwvzcel.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gdegrqfmk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gpnvqioup.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gkwcfgipo.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzuhgfli.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gayzsurmm.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghniazyvw.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/ggxngsaoj.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmgwzjuz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gmezwjvod.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/goqrecjsl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/goqqkdedl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagdaxqqw.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gikjrhekr.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gbgqeccca.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gptrowjky.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gvyytqtqj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvxyqurr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeqpruiu.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlrrscwl.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gholgzuye.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/goanszzet.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gmoyquuyc.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggivcweha.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvyxilox.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gjcuqhnkm.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccrthnht.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbivupde.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuzjekmc.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvlteypa.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/goocaqbvg.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaiwecur.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/ghfpwjjyc.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrnhmahn.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjdslbsk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/glzhdgply.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghncqviab.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagcdokys.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksepfzqc.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjtkxahhd.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgzzzuvb.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gptvkognl.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/guqptjnlb.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkvalwse.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfqyjgds.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppsesrke.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gztlcchha.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/grhjpwxnb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/giipriafn.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gruuydkkw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuzbvxvj.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/giimwbjxa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfiuzukq.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gqdghxjld.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnvyrpxd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhuhmqqq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gifcmrnoo.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gdnfzoldw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflwqclmk.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gdegvtbep.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gluthvilu.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjagsdnj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/goxbhbfbd.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixceeveq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjaqqocc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gmfwuiszs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvinwwan.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gksbgzssr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszzyzdmo.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gywlbhelp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpmemjpq.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvlurspm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gopjjjobs.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gixesvgug.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmnhdcix.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/grjpnldbn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtncutto.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjznijcu.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwcenxtr.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoukwoej.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuqoyghf.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gdwkxbujd.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gufjglwso.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gxmibmsnn.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/glfzcsfuh.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gygbejera.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqitjjlch.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gofetpcvk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpteeqdjk.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gukalteoq.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcjyivkj.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gkailpoxt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gklkfkvzm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gromxuult.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxwwpfcy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcuagxdi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvepepqct.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/grkclxzab.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gipftnuwv.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquntcuqa.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gthvgbpxt.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gklrgbafr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gtktperxk.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gcpyqoodm.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfbnouzr.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfjrkmbp.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/grauemjlv.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbbrketma.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyijobca.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzaqfiis.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gfrotmmpw.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gporgclqj.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gugjtxrnj.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gsnhstvwo.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwvchhrr.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkpcufkp.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkowindv.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/glfnegmme.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqroirja.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gpbrhvsjx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/goizigkdb.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/grdecfebn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gkfqnyjvs.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grvgkkskz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzlkkplh.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfojmbxp.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbklneqk.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gvimslyuu.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gqjfntwop.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxarxpguk.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyekxbwh.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gvkliwehq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbobgkrnj.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gghaifefe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguafkiaq.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gneyoqpmj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/guxvztust.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswtlsbln.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/glvfqhdcj.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxysxylr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gtsrvxcxx.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/grqzmmikz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzyeogsv.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gwspphxtn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbvfexmo.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gdmmrnchv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gqddpdcan.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gnijaizod.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gbswugxfp.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gjjjhwceq.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwlrtxbw.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gtlycidoi.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfonzcdyr.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gvbiczeoj.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmjwlhhq.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhipgvla.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdoaoet.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyeftgxu.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtbannsd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhpnmobt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghjfxmpab.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/garjywjpd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gizcvzvaj.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gabpqunps.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghunsgapo.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/geauqrohz.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoajbzqu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/grkfionuf.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gegrdyhis.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdcydmqfa.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntbjeeax.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glikjbqnf.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gvpchcgtc.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gtqcvdkyf.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gxehgnmdh.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gtdjouzoa.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddkpouoz.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gifcfowmw.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gtvmajorg.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdmnddoe.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gledqfgoq.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecufeztx.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhsvltlv.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gljqxcfbj.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdwazpok.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gukowvdjv.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/ganuwplrs.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gpdyhhzek.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuxaeygh.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gasnhlxbx.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gmtahmsqe.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gftctfwhc.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbtolrrb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjdoiwaw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxncyiny.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gzximntsk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsplwnqf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgdkcbqy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxrvgqcw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggunsvepy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyjgvbhz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/glstigerh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gqufvvydw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeofdkro.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gugagjrnb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrrycood.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gcsqslmkb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gvthbzfgp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfuvnsxd.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gakntjkpu.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpcbktzz.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gcbyomhfl.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gedhxcjsd.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gxvscurab.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gicrqohvt.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtukdukl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gmutdneke.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gfxmwicqg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszaeqdgw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxfsdinl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gpdzsdmen.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcuzyalp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gokslupqp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gmqbishiw.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlmwgnve.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjdcmdssp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocyjewbn.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyrosusb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyazoylvr.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatgkkfhf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkpixoqr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxsdwrae.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gztrwerly.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gulmbcnkd.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/guqjyqdgq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gjubeccxn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajrgvuzl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gkgsoxobj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/grojpacpl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gygwocpvb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzabykifk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzmjhhsg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gibmyjdoe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gjaxtblej.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gldwlmiga.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gqmqrnylu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gczoeexaa.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfxoqpgb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjetuuut.sHtML


<!-- 参考信息 -->