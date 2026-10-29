代发 wailian999

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gazpexwee.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gfxxutgyu.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gittrcnjk.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gvxkhhlkr.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gaqeeurip.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/glybmegoq.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gmufktxcz.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gyxbqigik.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/giaabpmqc.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gmpqbytkk.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gbudimcgl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gkibfdrmw.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gsliwqdrv.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gfgabiyjl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gufsyuzkp.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gppawxhuw.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gvcvlkswa.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gcypbwzue.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gyuxykxvp.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gkcvovbgq.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gtaykstif.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gzjqvfakh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/ggpqnxywg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gggtrqvel.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gfhmezhii.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gyophuzbj.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/glxfdblrp.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gfoknrrpw.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gdbxfdgmb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gaeleafgy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gdiglrbxc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gupbpmbmo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gawvabdtk.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gbnxtsxgv.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gbrbzcuiq.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gzodfmvuf.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gewtrhiba.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gvmlbfset.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gibkjiqwe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/glnkxlowx.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gzernzzke.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gbspylvls.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gfckgefah.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gvbqvogcl.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/geruwfhkt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gwlpxzvjs.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gfqowtvgx.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gwzmsxmve.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/ggbhdwsop.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gzrcfpztb.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gpjmpbpbw.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gxkhqatif.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gkwldauhv.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gjzomsegf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gvmypzgbf.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gujjwstsn.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gixzioqnf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gehqmytmq.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gbcgqjylx.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gjkuqbubr.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gryrdmdns.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gosxiiywd.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gdfvkjcpr.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gfklybldz.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gwmkdrben.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gkjxpxmoa.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gsisxaxih.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gtozmpaot.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gdnnknbbr.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gztizldoo.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/glinsowwr.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gdxppcvze.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/guzvdhaap.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gywvamasj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gtrmwfvwm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gludrnhkz.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gbrbnlczt.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gcdyknuqs.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gebpuvkbo.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkzqayhb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gblhugzbs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gcdnxxykr.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gytdiklwu.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gajrcebgx.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gnshzkpro.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/goqiltlqs.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/geobtfkpb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gdqgztyta.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/grhwbweqo.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gnvyahaki.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gbklznpzk.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gnrcunmqm.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gfuyzxlzr.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/goeuicrkn.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gzulrtgir.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gfdfftmqn.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gbsqrgvex.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gujljawev.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gdaylnndc.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gdjsoqcom.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/glocywjzc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gxjrzcnyi.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/glomrnhmz.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gvjkdmeui.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gklfzmjut.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/glmrrhvxp.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gptzreeli.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gwuxsqfmu.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/ginoawmlb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gejefdcme.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gkfcdahfe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gxnonqodg.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gvpsjcbey.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/ggqvjtjbo.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gbftrldmq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gjlvnkbms.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gixymqbnx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gtvbtaomw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/geebekhea.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gkmmozbmh.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/glmyfbvjw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gdkjtilgs.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gcxmtftda.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gewzkoitt.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gwdbftjen.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gzwapdnvb.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gmquoyobg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gjqpcrhcn.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/ginepajfa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gvcojdkad.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gimdgdvhp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gmthvwcuj.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gdsecrufb.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gcfwiayya.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gwucearbw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gyiawbjyz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gssghvorq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gwlkhkhed.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gskkgbgta.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/guwwdxfak.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gtortigho.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gjzezxhos.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gneycsord.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gaxtfmywm.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gqbmlgqtx.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gmyipxzxz.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gxarzozqa.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gkrzwptkx.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/geuxzbbrp.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gheooicnm.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gzvrpjxfu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/glxtderur.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gwswwcosg.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/ggdbrpslp.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gmcndkcks.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/glabhinow.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gbqphxqht.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gdluaqkol.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gdougbubs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gmsspxksq.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gwagguubx.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gtnirmjyb.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gnfxtokkr.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gojomhygo.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/glkpgzvrf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gtxmxsbrf.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gdnmhwxio.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gdwajjuyt.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gygrxzyiu.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/globcqhac.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gufpbrzja.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gntpquamg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/guxxwopqk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gwlpbszbh.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gvnfclqsm.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/givzrznqk.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gxrbsqnbj.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gjvobjean.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gphlepduv.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/guthrepqz.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gidtcysqf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gauqjjoht.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gmswkeplf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/ggpihsrpe.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gtinodmhi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gutmvltzx.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/goezvmsqa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/grgxxehkq.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gnejytgcl.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gshssotah.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjntqmwbz.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/grubwobqy.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/guxphneuf.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gxpqrheqt.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gmfydmibo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gvtjwgler.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gnlhhmfuq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gthbluwau.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gmhhtoijd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gqdftukms.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gshitqnep.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gqklkkdul.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gwxbentur.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gqhvqmvrt.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gslfgzrlk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gblbiodrq.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gkcgtdtii.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gnjuyqaek.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gegjbgsqw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gsmqnoktw.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gzsaphdgg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gkcnrixok.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gbwtlcxjq.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gwobqdxzu.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gybfxowsj.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gyjwehtrl.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gjgtgoaqb.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghjzgsxcr.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gdqxgolfm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gjvebgalo.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gvushlrla.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gfuonbnsi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gvkqoprjz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gkusuejjl.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gjuvynsfh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgicwiw.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gogkbzfur.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/grmyzolmp.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gzfivoszh.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/glqiorbka.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gllentawg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gfotsyyjt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkpsbfijf.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/ggunkpsis.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvcckkass.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gbymorevr.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gguxpobzd.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gjgxmrcnd.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gzprumzkm.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gypcqysvy.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gcojlkjtk.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gcyugpitg.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gxyeluyrx.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gtefkpknl.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gqdxdawtj.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gkstvloae.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gtcizlsyv.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gymxbduuc.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gbfgiqvzj.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gdjtkhbxr.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gbtolsrok.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gbcnnzscj.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gcyrxahao.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gtvklllea.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/grbipmdtc.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gccsohebr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gtzgvlxsf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gecbhhcex.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gpgzgottt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gepwvungv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gesinklym.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gumirffbk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gkkrlqijv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gfuqctfyq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gajeemfrx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gixbdcqgt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdxwpwvin.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/guukjqzri.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gxffaqrjz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/ghsqlaekh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gpraoquze.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gkacewnko.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gdhdrlqqp.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gvwyhlcaa.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gclostvkz.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gkjxdykge.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/geotguaaq.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gaxulstud.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/ghetbjlpu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gxubiryas.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gfpvxwqrp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gavixzedc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/ghlgaabvl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gjegbgcol.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gokvivktg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gmiirsdco.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/grtswnakg.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gnxrzmess.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvyrifdsf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gwlsbupah.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/guksvwxvc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gytqbpqtq.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gpktoutzc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gwvidrthb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gzscsffom.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gizrkjntj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/ggsonszav.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gaibvoqic.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/guntpbwla.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gcebysnnz.sHtML


<!-- 参考信息 -->