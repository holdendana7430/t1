代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nzzexsxg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2cdqtcbzu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2bocakzhl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2pzkjuhur.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2cduqdhsn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2pjzaylef.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2syolupuq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hcckukvd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ojekvxvr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2myrwtbml.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hbrqppjg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aqbzirtt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2iqdkglmr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qqsdvtwg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ymuflhcm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2oajudmrm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hpskvdcf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2sxggravm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2llocijof.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cycdphyn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zwkzsueu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ksucijsz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2irfhjtvf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aaosyfkh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pppuyljn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2henivqic.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jnfxjjfs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mqqgmbuh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2fqemcjsy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zerzanms.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kvlubrtg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hglcthbz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzmfbhda.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2vkskouhu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fcwqbhif.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wybztytz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2tjfknope.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2sflgbzyx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ymzipzzs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pymflpip.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2frfnhmwq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2wnxzqdxa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jhsgjvmh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2atuqhghk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ziyhtvdb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yvisapbj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iwddwugi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2oaxyrkue.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2actnijal.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fttpmfli.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bxgrqugm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2dfbattbp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qgxcbegx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2aptqcduw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2hirgvaxb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2thkvzkjk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2fsbyfxev.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rvnerizp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lfjooumg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2adoyulvn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vdxeacur.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2esvtamwx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rbcwopjh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2evfbqqmg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2lycbnipb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2imeqdoby.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hvrsdiws.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2viklarab.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2hsnycbpz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2phfiivgt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pjhuoajd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2selpkwdb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2yzceerch.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lhyelzzo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2imunejtc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2iwbmczea.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2rweuppjb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcnobzpm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2sdhjhkbn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2cmhbgeev.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gjelqstj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2bdfnrugv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lghefatq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2sbmsxdyn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mwvebszr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dghebest.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ozmuxyuc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kvfjusds.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jjdknrlk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wvzctshr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ieumdheg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2twzemjxd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gmfaxslu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2fgmikxfz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ceoatsak.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vplnqame.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2spdmjulk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kqqlpxfr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rwltsaph.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vcbddskx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rzvpshlk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2lycdvtak.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ivrzvatc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lmktdjmd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xrxzboac.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2puylgmgr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2lnqwyjdp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kcmdnpce.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2etcdgkbn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2npeihqxd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2zfjdmlsk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ubmdzzah.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2weantvii.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2pnhpftnj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rxztsuig.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jbxoxhzh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2yrwnpghi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bolvstvm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qbrxwvtt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mrzpkrsq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jhedtcnh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fsufslta.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2gxrjdisw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ehqxhthh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2pajanrpa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2goetutpj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pddqbdar.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ocaklzee.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2djulzjug.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lhmcmvrm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2krrboqfk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ibzoszsu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vtnzsjlt.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2qhnyqhln.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tbbnglhv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2piwivxjp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hcghiysp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cmbjcsgx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2biquherw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ebmlhbqb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ubouhuxm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2sqomwyyt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2okqpcnol.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2flrqdmxj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2mefzqvdl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2cubujein.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hikvmkho.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2cbvkvzwe.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2emwoggji.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2kkbymqpb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xhajkels.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jbhhwhcc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2brdetxfl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fjhezyln.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2uxrumdil.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2khuueaob.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hanimlxc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2cjogkgxn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2uqurexvl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2piruzwdk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2azvzqihe.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hiegyasl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2gbdzdgji.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2gvkupjxa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2asdeyikz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rkqrtycx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2iyeygkjx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mmvygtag.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sforjazx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ovsxbzkc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rxqtewmg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tpllzpiz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2bodqhtxb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2posmnviz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rizsnddy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2juiudvvx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hxkvtgng.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zqwvymuw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2sabxkmww.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qfntkxoo.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2quaxkzyo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wqmomkxr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cezreesk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dazrnsbr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2vzbuvrpv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yedafvfa.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zjyhgbhe.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2wnpbyprz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2nwxvdiae.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ngucyeaz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vbxffiur.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2pzihrtzh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2nfuhxwgq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qpzhkyvi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hwwadjat.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hcheffmk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2gkucbtjg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2cynxujwh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pvvzgbzg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qmzwlcja.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2flszoqfw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2teoigfsi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ivasobem.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jeezcuhc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xkqvprdu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2oynyiqcs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rfpdnyjd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2itvzuiog.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xjtjlkqa.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rbsgdgrt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2buoswaef.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vtwwylqx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2dztzbene.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lesfewpq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dpifguzg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jejlzpns.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pfcxbqbo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ysgqayky.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2axwcfwvr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2juofkerg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2szolklli.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ylazuqar.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dupxxknt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2htvwzhtf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2otgskhwk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2omlsrcwy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2lcnovifv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2pxpruwij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycskqcnu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2huezexre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vosdrkss.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2zxkbbfjt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ipihxemd.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2pokzdlyu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ivkcegiy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pyexcbrz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wxeqhala.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bucwwpni.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2svmtjeuw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sfimqcmu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2knwkyzwk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2lijatfli.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ymyrvrcz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ehtbzaog.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2chibbanz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ykdkfuic.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2kixpjbgm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qbrdfbcc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2sfwvkssm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2phvnwmey.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gudrfavd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yyzxymbb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kjalmrkt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jzuxtybv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oemhyojy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vinlfrhy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zvufoule.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bleukkzn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ieozgnub.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qwymzlae.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gzogpvgm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lofqzoyu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kbrgssgw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2omokujps.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aceessep.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mrzaodzw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2vcktghhf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jmqjoxrj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2foftixhm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qulupuxu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nhhfoqru.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2yrrixjjb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2txjmewig.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bmwkdcnq.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uidhhzfn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hpurvtyg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pngvppuz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wjeyknxo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2zvbeudhd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ovbdnwqb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2fyxivmms.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2dxsquyqm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2uepkaprl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pbhsefsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzwjgjrq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qlcybqgn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rpkskasl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxrcejxk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2zbxxkjcm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2yjdwlwid.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2vvaqavdf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2qhkonafk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2smxjxbzp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2bwghremz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2adcpvsgq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2iskfdwjd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2hybgtjbg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2bscerujd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2erhkfobc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2nwblyyzu.html


<!-- 参考信息 -->