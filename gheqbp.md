代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ruormyrz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hjcwkaps.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rdksiepf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3irctsuev.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cfyxnoou.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3brmsjcwe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3siimmmyi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hfqgxfjk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3htawueyf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ihbukdvv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3gomjixdd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3trlmrlfi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zxbkytfo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tmxxhpbt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xshkoncl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dzkphuxc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hlsucddx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3eijjwagj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3tyxdguhl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ldlskdus.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3weyhwfzz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dlelgwbt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ifnydubf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vpunbifi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3veboymlh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3cdurwpbp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3eqvgshhj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gdqskruq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ynxcvenm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rjlucosc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gvtapvvd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gjskpqrp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wjqrcfhw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3fknugntx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lnnbtxdy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nvkcuzbw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3widsgnic.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3gfhvcckr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3hzrpzfre.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ghyjeswg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3gkybnwpr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3kzlorfrb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gnmjryeg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3jambwkue.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xmqtmysm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nirffrvm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3knekhsym.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rulrmoxu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ksgkfsrb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vvyilvjz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ruzpszgj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3oklinelm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3debowyoa.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vrziwgwe.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3arskacds.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3xsvqfmjb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3czvyzwwh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pfmhojfq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ututiwjw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hacnyhul.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3evrzphgs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3domxzggb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nsrwtjpg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3hbpeyoez.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sdlyqxzs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3spplcene.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ubttzfew.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3hmqbhica.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lqbbpndk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3sjntgfnj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3mfdukgzx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbjzfwdi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zcxkjgvi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3pfcjapcn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cnpbybhn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3amvvuivv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3amoeinsx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3funeyhzj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zsljixnl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lnracpcy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hlhxncfb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmjxccda.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lroldjae.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3hxlitdzz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3upgpgbtl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ixdimdfj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ngamyibh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3laehaezr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xowxxwxe.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3docqieyr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3rihtivsk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxlevfcg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mncgzlmd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uokkrgqe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uliylvkl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fmxhcbxi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ezmgtiob.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3sbyuueaq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3iweqkgin.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3jygktbnh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jqjiadhq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xpdlltbu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nlyxraxr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3phdbeotn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cjyneysi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3klwebypl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fcnyffkl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ynaclctu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tzwcjqxu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3elvqusql.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3dzfowfam.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mqgrtavp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3srurxtqz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhfevmra.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3lvtbhyxn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3gxpvgxoz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3kysvkwak.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3pyjiijmv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3oqkhmmpr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3adrszggy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nbpaxvya.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3guytiina.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ejrotklm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iiawvgzi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zueajyfo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3pomckcca.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3pmdefesu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tavqsmtz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3haeejedd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hdayfuqe.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vneinxnl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3dtiaurlu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gqjzyxsy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3cprbglnm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zcbbuhfj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3bptsemot.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mncdnrrq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jzgatbim.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3znzjflnb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3guetzavl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3vydjolit.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3apigkesy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3lmngbkrg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3iueethso.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3brtuqudl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3idthyjhx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ikwdsiwk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gpzggmot.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pvhcizdy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hhbnrfqo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tvyhomsc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wbyezwmp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3lcuipzsd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bbgnthwe.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xaaqwiji.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3txtqjntt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3plqhtstp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ivtecrhw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xkhybgat.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3gmgantja.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wuktvhmb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3dedwdsvx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zmpdrnfr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3djboueas.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tkvyrunj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hramywjp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ispnhtzw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xljmbbzx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3yyllnxie.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tjsallij.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wpypgqgp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3axauzdqc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zmhwbrgv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hzxcfmtm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3lbnkfijg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yxlfeqza.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcriijky.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3tgqrfoip.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pwcpprff.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vataycds.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3sjkztzmg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3fttaqacm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hnmjagda.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jchnllvx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lmxiolsv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fzxwpftf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qrqrxvzm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3fzyahdqr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ixetnyzx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xkdnpbyj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ejzbocrl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3iwkkmbft.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3kmoqlhsb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3fljfmeyo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3kxedkkne.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xhingzry.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3blrtdamg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3uyirraxf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xqwguozp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gsldtljk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wvyhejii.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xyuszdpm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xszjilzq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kfvwjwnm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3aazlbmda.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xhubroyu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3yddtviqu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ixkypitr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rquyjlmp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ftfzgdwk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3gqfzmppa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3tsshbcew.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hnzehdtv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nzltoilt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mitpzzoa.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3amzvacju.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nyygzqbb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lfoakpfq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3usedjmhd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3opuhdiva.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ffapltlq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kzwaxbjb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ushklnjy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3youpcscn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vnjvlewk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3tuyofxnx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3tybrepip.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qxteliwn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3cdjnmowv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qcczwwll.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3iomgjcoi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3yeqyxbwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssgcvoko.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3irifodsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqtgvuaa.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3kczppqdy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dzwplnqg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3hpyfltkk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3wqzqrrhi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3whjonihc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qkvghogb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pdzjrlom.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bltanukk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3npksmntu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vlwipmfr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ohdvxnqk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3giutgxso.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ztqfnqtg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nlilsyoe.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3svqsmucc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3twifaybt.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3elkkyvsy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pfwytmaq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3swigpdel.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dakqwanh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3pguuujvc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lhgsealp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3agulsxpq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xpguotqr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lateomzc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bukvnaui.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zwtwkrxi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pxnjhjur.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3oscwibtb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eokpfhfk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pxyqqqje.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3frpjxpts.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zivszytu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3brzwpixt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qrlvdgke.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3xjztvlcq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hllnunbt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ipwiaiui.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3kyjbxsvs.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ybuovliu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zalomgcx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ngqxtwsz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oofaocpj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ftmadnus.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3benoneja.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vnjwgnqs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tfwukxna.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xskwvlny.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3dtbyoksh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bslvyome.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gbelrhnn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zecjfdkn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ntivuast.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3waaatbss.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mqytlbma.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3yeqbdlzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pngvlxvp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3gbuewjwt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3qvvlxaar.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cjjojadl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3qootshmf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qmbbolvz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3zyfwhxrm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3kcdrieqi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vdkqkkun.html


<!-- 参考信息 -->