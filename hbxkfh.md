代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sehpfyec.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3atuygrtv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3owboafsu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rllcockn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ntrcpdqh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jitfzwlr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3frrzhbwh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uwzclpiv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vxrucqvt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nrxcnqmv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qgvleizf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3akpqdadh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jihhasgr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3oiwevaek.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3daccvhlp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3amjfckgc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3natcktku.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kkrjhpaj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3uxotzpra.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ipjwefau.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ptxqgdve.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hhwcardy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bdzdgiel.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qzejcisz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3frqkzfyr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rmebxoyc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3evnnekwt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ysmugvgs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3utarbgub.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ceiffcqx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3opfhgrqh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qxdyktog.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zljuhmqi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3npovyfpl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3yyspdnoz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3kcaleehl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bcllmkzx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ttwfmhkj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3imszjzfp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tawuygtj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kbxmzrsu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jfiziyyg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mgxmvakb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mfruxuvi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3dnsuayus.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qvgjwwed.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3skhkccid.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3pkywahdj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3oxwlbrpz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xhraxvfj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rehgtfji.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xhcuwyay.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wxmmtmkd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wsihyjzf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3agxujqvy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uzxchigr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ymylfqkx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3flyljdsn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3vbqdwonp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ttrvddys.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3weuzgzdw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rmtddmcc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rdrqhmew.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3heknfnvc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3udcnunma.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wwgrpeex.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3liywezbz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nlriarwz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tyswkpzs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ccsdnlin.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gqdzknff.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dliagqqa.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mstfxapu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3iihfbwgz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3hinzobhc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vpffvdfe.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dibomoch.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hzuwcmnm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lyqecips.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ysxnnnzb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qpsshrko.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bnvgsswt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3buybhdax.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qpkszlkw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vpoljatc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3smlcpvrp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lqewydyr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dlmzypxn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pkebvvou.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3yrulegww.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3upmpttxl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nubhiwjn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kqspbznd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tghfgrxs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3nhdzydmj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehlvphql.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xxhggewk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3axtsceuo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kyfeksgz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gwikacqc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ynqxjhyt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qshqtxou.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zqdbvbne.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ctukzhvv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3jrpxvvwk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wcgygepa.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dowdzlkl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3podwfcic.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3smxwzpgu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3aprnpdic.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3cahohljz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pyljbniu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3geemdfnc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mtsewnrm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3clkbjqbo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rtktsjad.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mnzlqvmh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ckrwofqz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gsonpuqb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3zmgqeqod.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vkevlsic.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3jfziwxxe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3oajegaks.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ixkdxerp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3tscebxkf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ztuqxjod.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3pvfudcfr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wffsdifb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3umuajsrf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3alsdgswk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wxwfrtjx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ycaoxknr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ixbyhxpl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tvzodtpg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3iwkaspbe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sslvzdiz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3okwamucx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vxxcgqqc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hdrrgboq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qnwkiyad.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3uuhuyrwa.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqgojxc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vcsufrpx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3hmjrwpjm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3pzekvyya.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3klbqqlwj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3camhoski.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jzwyszqx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nonmhwdr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fnkeifxc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3owapyrkr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3sslfvwlj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3recseoka.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bwstaodf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gdkxrawq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ignhlfgn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ldscpiex.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3xjpyeojq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hqnoodpe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dgwnrfqi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zyryghsm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jwtxnopi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3unmdpqpw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qrlinkzs.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3nrznasjq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mjpwyhbr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3fsfmaizn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rabopgww.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mgqwuiop.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3pghuioyt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3axuwyhsb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vqvmvlyv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3szjdcrjk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3duxfdsxj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3phdvhili.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yfzvrkct.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qnitdeko.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3gyhvwdwv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cegymudx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqeesvwu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3bomiaktx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3papgvvqk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hdqmxaie.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vedaugsq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3rusrzfcw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dkcjyahc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ppsipjcf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rpvpdeht.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yafbtsto.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rhgdjmtl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ppppgddb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hijduunp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3voesnhdj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3nolnmglq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tkxnanzo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lcpthgaa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3hjevnowm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3txhzvxfi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vdubgujh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nrqizglr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3vovfliaa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3xsjoqtwh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3dkdardct.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3emvjqghi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ftarvtug.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ebrumiwg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qtebgetj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3yczwyxmx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ljmqapps.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3buxytjiq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fwrfhvtb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3hwefamce.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jjqkrijy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ljtyjpfu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gbkxeeir.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dfrrykkq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bptllsej.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dphoqwdr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3vtwfrmkq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ptblkipy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ljgwpsxu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uxoiypuo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3dlsecwhi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3glwoyndz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vyimhgus.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nutkbzmd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mevjwupv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ddqejjyt.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3yjgnsvdr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3mxaiqahg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3trwwgusz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qkyxmwbi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xbtqpvky.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zdxacaom.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ndqjwhzv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3aoscsvks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ditmpgxo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3trbvjtia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctkqwnif.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3turqxiyn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3fyuqfgxh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3npioavwi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3slnoyjad.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hkclwdxk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3shatcaoe.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3uvgpbudb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pcccyfzl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zrmjzfuq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kislermx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mrbewhdj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mnrgsser.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3cmmzwnyq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3vgxjbxtj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nsvbsfrk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3opyzohnt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3oxzpwnzc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pewgrmfe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oebykpgq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3rhodpbna.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wehoxkbe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dwccprok.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fvnadvon.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qdtuxbcv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qznqzthd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rrudnxpr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3oeceeyxu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zlfkiikp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wmauabvl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bwpgzayv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3efukbkzl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cujlijzo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rwsljdsh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jqrablmm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kfaussqx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3jqwoqdkb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yfjonbft.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rgkpeyxi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3uwugtcmj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wcetqjef.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3afgwqvhi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3iijatbvs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bolprjrb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lecbbhml.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ospshevi.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3syzdpcup.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oxzlodkb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3gtofxmon.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bgtutwtm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3uffrxyfl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3mebecmtn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ilxghmjc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3psiwluee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owvwkdmj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ulpognwl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3bxzrzuir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edstbjvq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zfmsyfsl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3enpulddw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3tpmfuvyo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3rvaycngx.html


<!-- 参考信息 -->