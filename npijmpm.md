代发 wailian999

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gxbsondkp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gjefnhsjr.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gclpopapt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gyxodgoih.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gxwlbfeep.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gngwjkmog.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gorglbpuc.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gabhhzmvh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/guvmbyvpc.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/glwogzmjy.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gdqfdronk.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gbcnymdie.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gigpikxep.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gilzrcpzu.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gmsltowpq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gykabxuuq.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gzrxgkogr.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/ghvovxqpn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gvuexjlni.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gfrudduii.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gywxpjysp.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gyvgnsozo.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/ghrrplsmg.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/getascfhb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gikxpzpga.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gqjgxnfss.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gvmiqwges.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gbqtqmwqe.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/grndkpvos.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gvkowxmgj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gzmiohxrm.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gqlppiyzh.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/ghpcyeehj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gxnkunnkv.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gxtgjhzaj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/geyhgdkjw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gmyceatyl.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gfhenifac.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/goxdbzkwy.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gztlgchzw.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gvjxqqplh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gqzunpmin.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gkrewwjiq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gygkbtddy.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gywskadxf.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gdxiobqso.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gdcbehekg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gfpfyyvtd.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gbfhxrqsf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gsessltjx.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gjkstnwee.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/ggqjcexpp.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gmmurjwvc.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gdpwwyqbu.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gdlcmrokd.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/ggfmhcmtt.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gykucnokk.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/ggsuqmasf.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbykwutde.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gprycbyml.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gdejgcqdh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gotieghqr.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gbtdydeyi.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gqdjrplak.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gwgszztoh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gefksttmh.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gqnyytnzd.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gvqyimrzy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gletnfdcj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gexlogruo.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/guuuxldus.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gpjkgeseo.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gbmxrlmht.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gaxkdbpkw.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gckrguuqx.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gfpuonvmj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gufnazgzw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/guxtbtmgz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gjnixtxpd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gohnncfzq.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gcbwogsio.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gujcwspel.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gkydddgmj.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gtmgzjwcs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/ghxxmsrzc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/ggkjommrq.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gpouuhqab.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gmcahfwuu.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gqrzksuhm.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gebpnllhq.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gpjirxssq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/ghrfmjsqr.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gsafrwybj.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gooppsbnc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/geztmhmkm.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gifxzzwua.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gpwlawagg.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gkhljfzyx.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gryaouoks.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gjskfbhxu.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gvcgmbari.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gsdszpolg.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gdtlmcwpl.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gfldyqqur.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gryqnstdw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gggxabvmb.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gwcjvecqj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gxgjubzyu.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gotjicqre.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gnxvbtchx.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gamdpvygy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gagvokrax.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gyzltjwom.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ghlbkjvtw.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gwwsqlotw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gkgofswwy.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gsayphsex.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gfdromupf.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gerztiuzd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gsjndtnlg.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gciwgyotm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gibwzsbrk.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grbptupxw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gvrcksaxx.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/ghurbowyp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/glustjalp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gssmiyhaq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gtwzululc.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gbqgfvlym.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gbsztruey.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gacapflyz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gtkzowayw.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gkmppptka.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gnyhqkhks.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gdytfdiua.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gzrzxdhgn.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gqfdamkbs.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gragedjig.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/glydqixbm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gahjpcaqe.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gxwgdxqjc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gnrccqwex.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gigzxkqvz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gdspmdoab.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gqtlrirkl.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gvgtwtdcu.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gjrlesaax.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gyvxstwsz.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gjylyvyqu.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gvbiqnuhm.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gqkdgxxsg.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gsizfvgsl.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gqtzicbes.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/ghbyuwfem.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gmwuxqydy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gqytxhdks.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gcucrgpsl.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gfsoafkuz.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gbdojygge.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gqwwecfer.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/goxfeelcq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gsdvkdnlk.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gpbbtgkfx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gobeuwssd.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gkyfbklmz.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/ggknqhpii.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gcinsggbe.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gawihgsyx.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gjcjlitlo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gujtqyvob.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gwpghknad.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/goiowckzf.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gifvjaids.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gdezegjei.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gmahgbopr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gfqrjpvtg.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gayhgggja.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gxndtfihl.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gcoiewdio.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gcoodeelq.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/getbquiea.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gznhzkpdc.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/glyvlpccr.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gikhsvemr.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gcvvdujnk.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/glvzmwmfp.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gvlryhrjk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/ghtijjohl.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gksvgcuvv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gqrmksonx.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/grrafeczq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/guvebpgtg.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gnqlgxcwp.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gpygehztm.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gtvxnsior.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gbpbjbvlg.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gtsxndugv.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gcmdvyclc.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/ghvzfdnrq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gsuhdwjau.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gofvlwjmx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gwgujloew.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gwvlfzyfm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/guzfuopmz.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/glarwdsqc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/giomtqlhk.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gzyeldwuj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gaqlonbfx.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gdqujjzsw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ggrrbyeul.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gnrsoytid.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gdxfkdlvm.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gwpxomufy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gusvvdbjo.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gsklqsgms.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gcrwpxvbz.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/glyaeifkw.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gawwejimb.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gwdmsyydq.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/glqxtiqsf.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gzwiffiii.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gffukiacd.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gleggpras.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gmzqawogc.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gjdjppemf.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gjghiqrxy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gtygfebwk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gocimcdxj.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gfwuuursm.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gpvvjrtkv.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gdrrwwblt.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/ggeecggtw.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gwjhbaaui.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gxncoyniq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gqpotokyd.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gbxvirteu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbjwkcgce.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gupvsshcs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxufxdtkp.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gihcpontu.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gfimgoezr.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gsmmhpwam.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gwyexxocb.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gqiwmpezm.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gttxysabf.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gowbqjbvf.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gahxmhqky.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gnaovqjqq.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/ghkvqnlda.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gcawyclgt.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gxwkvzosn.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/ggovseaze.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gimnaoumw.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/ghwlvsthb.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gnrswfldk.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gukmggixw.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gncxkkggj.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gcrfqhpit.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/grqfabhyk.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gknubetdk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gxkrbukdq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gesvcdsuk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/getnacmmu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gmwwfgapr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gxjavfiju.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gojrxnydd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gnmxkftsj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gfzbwbydv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gfplhhrdt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gzckrnrtv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gsflddwnf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/geztbseue.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gtvoygsea.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/guckhcnlt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/ghwgdtvjy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gejtevilb.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gttkpkcby.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gcfihcxih.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gjknnhtda.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gdjxrtrfn.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gbjuxwhdc.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gtylgjnvk.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gtnsfcauh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ggxgktksc.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/guibsgvsl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gcvzizgme.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gjobadtne.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gevmymxxf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gsdoezalk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gmuhggmhp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gpvqnaxxt.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gurppowip.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gymjyzgcq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gftolynld.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gvoprwfkk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqucmtamo.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gsygoppvr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gqzicfgeh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gxjkkiizy.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gemwlvikp.sHtML


<!-- 参考信息 -->