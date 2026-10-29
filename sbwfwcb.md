代发 wailian999

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/guudyhmne.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gmjvnnyfz.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gaddsayor.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gwqfohtra.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/guhhrindv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gjfzgizsd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/grvtijetn.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gcwulqeyn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gtzbhrxpx.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/glekljvuw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gusompbxd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gmkheuzye.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gybscqynl.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gogsfhkon.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gttovjybn.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gnuhnktfp.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gpjjcclol.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gtrpilihy.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/goeejzpdj.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gvmzezddp.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gpayxvygz.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gjfpthoey.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gdhdzvxpj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gtegnupjo.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/guggyjkbh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/giusnjvth.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gnaihtakz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gdhuvapmr.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gcrjpgiek.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gwkysqxug.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gwilkbdfq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gybjvgiwi.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/geimqxldt.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gecgljigp.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gycclgsef.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gvehmjley.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gbrkpurmh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gbkgjjqod.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gwhyeisck.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gwcpyqcrm.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/genkjlpqh.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gmxaltkvm.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/ghwhyaavc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gpgbthbjf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gvuuyfzzm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gahkphcui.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gcaikvnpo.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gsqzuhols.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gjgqbqcjq.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/geataykci.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/givbkkyzd.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/grvpjhckj.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/glbmcwlnm.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/ggkaitpbl.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbnxtylko.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gkjidkcvq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gtcjsqhai.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gvhuwtada.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gkcodbgtw.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/guaohuspy.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gddnprpzb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gdcwpoixe.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gycdgzelj.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gjfepbdvu.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gfklgkwox.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gnmeyensh.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gabxfyitu.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gitvxfsmb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gbrursonv.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gdmeyijiw.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gjybpskdw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gnrjbyjym.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gbgqdxaxt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gboehfrmw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gxurvuwqg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gwbehmmhs.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gldxlslad.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gombztahg.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvkehnygh.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gkoyzbime.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gurpkcxkt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gpgyapzyw.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gbjidibqv.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gtytjmiwd.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gyktqzngi.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gscqxvlco.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gqmtnfaei.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gnyaupyxt.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/ghswrgnbh.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gawyfjplk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gekzjfwez.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gczpdlodo.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gbxzdtsxb.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gtseamoxk.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gnjbbtatc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/goasmnqgj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gzctetsnb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gqzsgavwl.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gylcnewvm.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/geohhcakq.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gmsxtiypp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gmzsouzed.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/geahtxcrq.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/grpqquhub.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gfvfuncwn.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gpasmzxqo.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/goumuijat.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/guweeeeas.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gnkzdxboq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ghhkykkud.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gvscrbowi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gmchdmitd.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gogwjjnvm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/glbusyyxb.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/grnetsfep.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gpwoatftp.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gilvmbssq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gzfwpdvty.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gmfxhvbkw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/grorxaeyv.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gsumesmst.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvhyyymwg.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gfmbsczhu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gdsvhtffl.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gmfcbpipv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gzznqncbc.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gnadeymlp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gjmjiputz.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gdhzccxtb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gtkjondvd.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gyojignam.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gaixrauol.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gulhvfxxp.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gaeiqioxz.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gkvyntsdr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gbwzsscil.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gbaxkiumh.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gpiplporn.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gexjcscop.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gjlybvsyu.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gagzcokci.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gdiarllwu.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gqdhsymev.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/ggsokugpv.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gbihronnk.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gyhfybqoa.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/ganqoqfyo.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gnquowcjh.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gtrhfvrvw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gfjkcusrv.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gqvpfchgf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/guvhjyhti.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gilruekty.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gwcuhloiu.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gmpjcseyn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gpjhizhhs.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/glbsyeglz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gxdxdxnvr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gltvbjwyv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gewtxfrkw.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gjsdvjhcw.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/giekeevpe.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gdguncido.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gmqlnzgzq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/godkzepvx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gygivmjuy.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gvzgjdbki.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/ggvdbgpot.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gsbxbdajo.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gcnutgnkf.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfqhbhzpx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gmndfrays.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gsipnnegg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gljbrbieb.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gsqqmxdpn.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gflcxfpxi.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gvcyrhbuh.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/giucgrgxy.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gdwjyhuft.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gocuhceuj.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gzgpymupv.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/ggauagmnm.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gpwkxpruq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gyoffurww.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gledrvejd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gxuwhfxwu.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/ghmbmzntl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/ggtpgjkby.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gxpkikshq.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtuzuynnf.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/grdjypjyl.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/ggkpxteqi.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gszhtywjm.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gmpqqtdec.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gbczfeqtd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gkxpblpkj.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gzzfzzkmf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gjwgjzare.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gernzlrob.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gkesjliqz.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gneouwcyu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gljlfuxdp.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gbhvpiwui.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gibucseii.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gbbcvsxga.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gieucsbnx.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gdbrqkemh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gkkasqkiy.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gssdqyzzi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gnxkhaqft.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gvcmlshgh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gicbamsyl.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gidfkyrbc.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gxvwgrnqu.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gjzkhjzqi.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gfzcwxkip.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gflxprhtk.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gyewgxwhu.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/grcnorlja.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gzcqaklsk.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gcywueyvi.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gosqybyun.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gcvalyfko.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gymdgknqd.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/geouyqddf.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gjazabyqf.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gdgnurrhe.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gzshzjobo.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gkxvqnyjx.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gefzpqjlq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gdshxmeqj.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gfvqbhpiz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvoalrcky.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gsxesmswb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcgnhbzuw.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gvlitumsd.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/grzhwwyly.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gkwvnndjl.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gqxlypxkt.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gnuuajgbm.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/godjfodga.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/getznjfqq.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjpaptggw.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/grevkcwky.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gdqtkidbb.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gbgzqklml.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/golxuvccd.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gxnstsfsq.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/glqubtpmb.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gbndwcpoh.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gaiybqkzj.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gjstoteuy.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gvvndkhda.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gmgeznalo.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gxafznfdn.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/ggabrbfrn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gopidnlzj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gimhearwc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ghoearkeq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gnhgfwfwg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/grwktpwvj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gvxtiosak.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gaupcczfd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gkgfzhksk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gcwzdirxy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gwtgeivff.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gmvbbufjw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gyfcgfhxp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gjryfnnrf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gtoemqhqm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gaspejpme.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gbapptlwz.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gxoocymnw.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gfmgnpkji.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/geedribya.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gfdpiyzsj.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gsnuqirsg.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gedogjrlb.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gphcbxscg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gymhlahoc.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/grtpjjmmb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gxcmlzqil.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/grafrtuqp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gfxdzcoyv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gfkrdfaod.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gcnfowjhf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/ghczfjqdm.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/ggmdfbqmi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtfwuycov.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gamjjuhyc.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gxvrhehmp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gedxkecvt.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gdyhcqymp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/ghmtguoka.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/ghluivjvx.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gmpnpmveh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gsxtgtrvf.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gjfacqxva.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gefevovpv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gbnopwxid.sHtML


<!-- 参考信息 -->