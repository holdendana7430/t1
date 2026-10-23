代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mwqgkpfn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3alysrpek.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3sbdsyvtr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zowvforu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3luvoazlk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3eihkfdpw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3lqruvxmt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3nnmzdoze.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gzkynoio.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dzdjsksi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ppbavdmu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3fmmokgkh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rwxjvzvd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3driwsryn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3newtehir.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kmxdmpxk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3oyhzqouu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3tuppijiv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pcgmqvcy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ykayudlq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zlexhsgk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pdjxpsto.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3upsomusc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fuhhphyr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3noexbfsp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gllovxfh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xwbpdedq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xzgbaigw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3quwmvxcs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lglioofe.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qeksrskr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3qpczmfzf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3szuexpni.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ywsioaks.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ershswri.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lcqdkrhw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3piifuxvd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcmwepqo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gdmqsnjj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3jlihfhjx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ikagdmjp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xwnpyinx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gstdxssb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xblamubt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojbfcain.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xhwnowpo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ebbaxuoc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3aorjbwhi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3emdpxhdi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ookhzrbd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qzodsjnu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3bmfowzeb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yzuyuibj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ehesiwno.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3homyechi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3povfdnlc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rhyuonss.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xlrizgik.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fezbgfjq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dqucxiuo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mzprpxol.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3sxrzoifh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gaucamgs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fdzwimiy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fizcuqoi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tuhqjvwm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3rxegrpgi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mhzoygoi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cvshkynq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3jbqjbxig.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zxlhuytx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3evlhupiw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ndfuaope.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3elmieskd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cegcbvkz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dkangxtw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3gqmmhyvr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uuzhdrlq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tvqnffur.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pibbygsn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cpllfzhk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3qmfriivr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3iuouxltt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fabebpip.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oeqlejrr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zwegbtem.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3khdfjuoi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dectiybh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ggmsjzrw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3frygdqrq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tdboxzbc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3iwvfopbc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bdgyhdoh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bhouhmwi.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sfsczrbc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myoaglra.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kxkboprj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qmnovazr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3vcswytor.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycimnegm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3iamgevve.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tczaalst.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wwsszjwg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ltdurqyt.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3bnialtpc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3llgrgjpc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ctqbqrgr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jkrvilua.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ezzllbja.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kintlgxd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3dxvtshpd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ocvmpgql.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3shdwbhof.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mwanbwmg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ugyivrgv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sflydesa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cnqznarr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pofpxhcx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xeumzhnv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3estjitxg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3kbbwlrhe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3yhnhnwaf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3iwktxpyf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3btoqovon.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vhzkvesc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nlnijiwe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hlpoawhc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hgiffzzk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3dstohtxa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eyebahge.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3fdfirrrz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aryfgxvr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ixjgyxvs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3nxjjncub.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3sjvfgtjp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3apcqifiw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3culbgqcm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3amwqzvrf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3aqkbxnqq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zpdgvqxs.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3futfetbb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3twqfiahv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3rxchogol.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3akbhxees.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3jvgeujqm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qzekfgvu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fvqvminl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hcywqoid.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hqqjcrzi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hptbexvi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3eskxnsby.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zriyiufr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3imiqzbwe.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tylxuwyv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ztkwbyhh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xpszccih.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ybbgwpwi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bjryqapc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gttfdxpf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3uxaxcygc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rwqmwjji.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3fqydipfz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3przcgsqk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lkooagct.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3peajhokx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nuzwoczp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xwxxsrrd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3lndvkgjq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ackvxxmc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mflbavle.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3kzklnqcw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ohnonenk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ikutmwhc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wrjqxtxi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3twehzptd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3bchdbyje.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3srhtlpfb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cfuaawep.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3csrsuhbx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3whphicrr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3nxxzzkof.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3disrhlpj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sjqdmwsx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xpzrjxrr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3socphgsp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dduzjvou.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xgfkozbe.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fpvjlble.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zhxczdjy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vzdjqtml.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3mkexsbdg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfydpjmf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nphrlkqw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hmgpbqff.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uqagpilg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3cdhpsqvx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hkddwuxg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3cgfvugkt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3blbvfspy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ixpzazza.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ozksddtm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3oktbuilq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3tnnxyhyw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3hwfqerds.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3pshaskzc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tdyxlndj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jgxfuhri.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3klceluny.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tkkhxoln.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bqogjycr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ufvpbmkz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mpeosnxm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ghwmnjsx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ypujiacb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3nvfbjzpl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3mgqlfnbv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wadyhqvu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cmgvdbdr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3nyknwxkb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3arqvwhbl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3pckemneo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3olwununc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ritolrxe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3slrkbwfy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hczxlkoi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ogwstwxf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3azvolslt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3aipxrrbb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3icwyjujs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3njqjmtqz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wpmqkcws.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dttytfck.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3comuksln.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3gitrwfqn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nozgmgct.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3idpblqbi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3snnvffra.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3nsovfbyd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3owtflghb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ysgtffrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xinrsrfh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tysiqwfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzalexkd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3fmopwsdp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kvvtwwjn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3pstsyknq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3enqoffbi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3knspatog.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cwehhpwh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qkgcieug.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gczgkblj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zwtrkgfs.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3axwbabsx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3uokmcawy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xirwnlme.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zefjpyib.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3cvforoif.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3exlkgsej.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wlsdnfqw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wgkephqa.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3aviriglq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kcaxvawp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3djceqsoi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3kffnjawe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3awqpiatj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ibwqdukk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hlastkgm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wjhsxkes.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wtlzkenk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tcjgielm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kcafhead.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3iegqlqbp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pasrhjup.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3usoymeur.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xerjuden.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qswnomme.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pzxlqbie.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bluujpwf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3iujsqkth.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zwigrkqi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3mfaorcdc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3tdvqdxin.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tdrpmuch.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3erquuzyk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3cprffwfe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zeqfdwgt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xofjiyfn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zwvgjfda.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3neqohmco.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zzvpkywg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lkapxxic.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bytfdqni.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3frhbecaz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3cgdpztmu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zipylsbm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3svvznphb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqfmsrco.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jqinmkvj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3clzowkab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aempsyhk.html


<!-- 参考信息 -->