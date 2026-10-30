代发 wailian999

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmoobhpx.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/grrvcwbbi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gemmwuaka.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gffcsfzfj.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/grzmsivbg.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyuijiaa.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gzlmisopq.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gowoxdpui.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gtpddxpzk.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gbchlpxla.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gsavzmfye.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/glkxinptm.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjuouern.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnrjvnjr.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gmluuhnxv.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gixqgwpek.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbcawlgg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsanypxm.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvekpsxej.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfswudbjj.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gouecmgok.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gufmgakod.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkgwjdvc.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfpbwidz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggbzddsno.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gberkbwkf.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxdiikhb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyejgdtlt.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gylfiusgr.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gbajjxwac.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvxtyxzb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glphdtzjd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gzidrdeti.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gzxxufsml.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/guzbqkore.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdxblmsv.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgdjvqmb.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gushxuwzy.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gfhazpxiv.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gtwozgawt.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkwevhwt.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgcwjgii.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxnzjwfw.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnmtgnhm.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcjhnnfb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/glucmftoh.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gimlfxnug.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gdtiukjib.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gimfbbolt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/guvjcitwh.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gawsodeoq.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gndbespav.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmdlwjwp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graszqsnd.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gilhknqgy.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gygdxnvyi.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmidrvjg.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gpagzzeci.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfegnhrk.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gbqpxkmcw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiettkph.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtudkpra.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gqciqaukr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxlsdbrx.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghleqgqba.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/glsevzlef.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/guzdocbhz.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkwpjdao.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggmnbuxnc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gosondftn.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gtwskbhmj.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/ggkmeyrsu.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdekqgxmc.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtczhqla.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwjlqcud.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grsageqyf.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gdebfehqp.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gfydtcaqr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptyvpvfx.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqfpvjwu.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerkidmhb.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gurxvehec.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgvstahu.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoyxhtdt.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrdwtcwn.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlagtifd.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoedwovu.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzowwkbct.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/giwhiunap.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gyypaznnh.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gukeazwjr.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdicxipti.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkwfbdrh.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gigihxtcn.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gseyfexqr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gosbrevlw.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/giuasczyf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjgememl.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gxwrnrxts.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjldrfntb.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkzmxilz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxxgkzlw.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpxakdfu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/getjzirpk.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbnkwsxo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjonnbtva.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvslalwxx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gyoikyazq.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvzaexic.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghzijbpho.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/geizmlixf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gmxcdebek.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/ghonqpkgl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfxryrta.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gcgiicixz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gggidsbfv.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gdzvrdqmg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtjagmlv.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gvwjtjkvj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuxvulxm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gitwlthcr.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpclfkdc.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gihunusre.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/ghmtjrovi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/glqiloedp.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxidajzqj.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdlvjbik.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gzlepzcml.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgpzwogv.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypobxtkn.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gelfrpymn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gduruibii.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzwrlgci.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gplzzacad.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gxatpujbt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqhncuaj.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gydatbeqt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/goxwmdwed.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gvxdqhifi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsilnlsof.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gwwrbwdnm.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/ghlbalnes.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gwfmigxwe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gpfcjeawo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyudadog.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gybkefygg.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gwaysnzgr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdybhkah.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gwafmqtfy.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gwntmwirp.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvsvbzzm.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcknguzrt.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdpsrgaa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gekunbvwq.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbbyiihp.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrsobeoa.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gftosxrkb.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/ggsgkylyj.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzckqbba.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gugnievxz.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlvlggms.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gmugsayah.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxcktehm.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gsqikghjb.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjvrnqdrg.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjovdgai.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gruqqjvki.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyntopjfh.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpveaafo.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/ggjdmbwyr.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gycicrrin.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/grxacourz.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gahtbiqam.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gshpnubnu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjynrjtcs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhvkxhup.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/grzgflkol.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgeliwso.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhbomky.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gilcyoiya.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/glljthdyc.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gjytwdkmq.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gleczaadk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gvywxrios.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqmxxwqe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhbxnsik.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gjrdauzxe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/glyskdpfb.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gpupwobbv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggspyqqzd.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzcsqvzl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gaynigkxh.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gglihrenf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/glifntcxq.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjeaylnr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizhkelue.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuhmgttl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gnicodboq.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gniqiumtw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymuovhaf.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gvtvxwaqf.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhtmsdmx.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/guueocxbw.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoaexmoe.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gwwcjxtkz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfnldwan.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gyaknurkf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwoxbftn.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhlaxrfh.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gapjzzgxc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpusvttha.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/godjdswzj.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepjmomcb.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gutnwcxhw.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoajzacr.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnlzsihy.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeqswuje.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gutcupkmy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeqcdjao.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gngtydvwf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gukcizzoi.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gwsyyftgk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghqantwtt.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrexdjkl.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gufjqtgdj.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gvjnvdncg.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gsjdipcya.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqtypzhn.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcisfqbsq.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsvoclby.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulhhwhwb.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gurlxdftr.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyzipnjb.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gknhkpqgz.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gptlbsmaw.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goohnuqji.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubcbwngy.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpkhlbog.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtixsocb.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmukjqonp.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziwrltqo.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gbpfmxlyv.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gokafvdyt.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkwzrinq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gsvcapmzl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gehlpydec.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gvewgzhzt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gplbgtlfp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gkxonokws.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gcnskusxx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzjftzbk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gmvvmgahh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gruggnifo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwynypsiv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/goseclzuo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gdjoaxxbj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gralvwclk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqppvmhu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoccrvgc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/ggpqdzbvz.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gqotoxwyg.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/glmzftufs.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gzbitypod.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gceaxdnjv.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatagxyfx.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzlffpjd.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gipgickut.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzqywpjx.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gxppfxmnv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyuozlbq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gengxkoch.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxzhlnsb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/goibhoyoj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwuavtxc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwwckxhf.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gvaowzqgp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnenqgwka.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gszptibfq.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoftpury.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofqtbehb.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqoagkgq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gpltjavzx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/grhixarca.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkptmdne.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/glvdkneem.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gvmlzuhzr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gaajyxcxx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gevmbsgzs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gbpfzxycx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmegjzyn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdfxkwqj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssbkcvyl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvndajwbt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnqapeai.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/goxiufmwf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfqitnqe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gefkzambh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/guixtwqsf.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcfhtnoa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gcihtxbme.sHtML


<!-- 参考信息 -->