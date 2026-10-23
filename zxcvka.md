代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yicmugrl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bsgttsie.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gxveatqy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3siackeia.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qeywpqfx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3enzqhsuv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hgdthfxd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wmctzypp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rdzhxavo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mnxavfeu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3bnrcxdiw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3bdxttgns.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qcjqhhiu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3lhyrtupd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3oylhgcif.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3xqgngwux.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3pvcxnjpr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mwuqipqq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zpnurqyf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qemgrkoe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jbtzvvzu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3oxevjuvu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3htbinnhi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3obqaijjg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3sqwtfyit.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3oeshgloi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3erxfcjdi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xbphgtck.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fijjrlhy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bkdgssxr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3aatfpcpa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hloeddsq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vysftjsp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3brmmnkfq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3irobnuzp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bdtxrjyo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3efxgajgo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3breikcnn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xvksmysn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gvxbubcb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ewmdlxew.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3pttrzmre.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mksjijbc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gzrfviop.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3smqudrdi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ucklhmks.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tlfwhyxj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ngrrsnsa.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fojvdcpa.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3trpqexga.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vrdnonjj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ownxjiro.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hiuqfnid.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3woqqroko.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3irxlewng.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3bdjbgvfk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wtyvlgci.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rhoaktuj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3uqvhdefz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zvmsnqft.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3landnrll.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3juxtxfwq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xsxkqhtw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vzsqqefz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zfxgmkpx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ecrpxbad.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3njelvhdg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3aeiqdflf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3mrbuurta.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3jjutlhbt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ennhzpub.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3budqpxmf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3odzkidqy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3jiokocpb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gwkjpqzy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fhwwztms.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pfujnces.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uhsghtqx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3afsidzvr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jpjitzil.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xvnrjfkb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cbvvqjfn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3nzshngoj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mijmyldz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mucrtalq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3jkgmvtrf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nvnjbjup.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3detzqryh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ujfsvwpk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tctwdrsw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3zpojzzeq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rqwacfre.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vzqukzsl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3edyprfeu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dazcwify.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mshjctme.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ythcbyyt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3fwaguygb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zpffukhe.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uqgfrats.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jzxtkcpy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vtyestrr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pciffqsp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yrjmoymi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wiccdoav.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qbmmegrb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3fwoxoyov.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3exblxpsk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3aqpbyjte.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3iqmztmpq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yhxglcyj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jdwallnd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jznakkaq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hhiwqpme.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3qxmrhlhp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cvqmsduc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3vtbzpspq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qseiqgbi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qjknnrpw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zjqznmxb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3whoiynpe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rowbjhwt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vtnyfgah.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jatocvsy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3sdazvxca.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3fldaedzq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ebxftnjx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3sgcsrsjg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kpocapbl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3farllkio.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bpvzkaqa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vdiaqein.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dgwolgxy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mircicgz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3expfqcjv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uwqweucg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3sqfxogim.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xowmfgwe.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3tbcedauh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3comownag.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hszefkwt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3nrgyexhy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hohzsgia.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vyhqiunn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bnhevqoi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3luhuqmnb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tqgezouf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bvgzaouf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wbaxhadd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3eoydmdfd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3epflqmak.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3yzzmyqkp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3fkxxtxrw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rnzsdhdr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ebtnrncv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3codsjaam.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3glqjoeie.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dppmazhf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3eckktayj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dcxvajna.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3lhsreaem.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bjxjjvcv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zmbjtnyu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qfuptwsa.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wcknuvpk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ztuoqkcy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xqgghlsn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3owrdzoug.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tdhebeuj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jvnlqimx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3souakbkg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3desgatvj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wwlqwrdg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3spsxtqwr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xqbmbyjz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qhqcbmtv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mehifekh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vmlafqls.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jrqgepww.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nuhywmxr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jlotygqm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ygfsgxms.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3judtiuaq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oafvplqe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gavulzue.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vbxlwdai.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzxoolri.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pgykehrh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lcennbax.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3syubwgsy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zzqokgde.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uovvdhym.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3puykuzzw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nowvjnuk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bmbkxzsq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ezoqwgvu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tqlgqxiz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nofoxvth.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xytjppve.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kfmctnrd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3lwcsgydn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3mecwlsvb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jhmqzqsu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bvdbhrlg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3iueqdcxu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3tzqhevst.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xeukywnx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xqunhluu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3clfrbthy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3tvyzpwka.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rawynuzn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3lftojrxu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ncdiqjcv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gyqwchnn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wlqutykg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3gztklbkh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3esuqnbez.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ffrnymjm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qnochfkc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xfxobktt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3opztstrs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3aazbzpfn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3chfdwrje.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vamigqgo.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dubgkaiv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cpncwkgv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cxkynlrp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vlaesydr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vmznqqlr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wzvvbawq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qtscoeot.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aarcpwzs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wazycnzd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rsejwjcy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qmdifzfc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3opprqwlt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mhzldvqd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rzjxnsqg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xxduwoen.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3teydjgjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiqrhwtq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tgcspxrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iheokogz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ciqjamnf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fyjaqqxw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3uprowgqd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jnukwqgv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3umonizah.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bnbtiuhq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vvzjkzkr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3grdztquh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wgzqspij.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3clnhyzuf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xgirmlwl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3mbupknyr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zorsufeu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ggiyrshb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3crfcavuh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3akgmzfvs.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3hfippzjk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fnwfpcly.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zawlkydb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mozygswl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3oirhzlhz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wogcstop.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qatvqubt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hduzceeg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fgwfcihh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3yzlsgkkh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ekynfreh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bdarddqg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gtsegsrm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3boenjiky.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yrkatxui.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lhpiqotx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wodjadyp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mwajxelq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ccdonrqf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3zllwpxdr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3djdkkwnh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ddjcwsli.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3kmnqezmz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gpneyajf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vveywuhb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3rzphmokv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qboiroef.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vsfutsrh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3knzgpexy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3oxhgabgv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aoiyxerp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3rumcjhhk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wecebiwq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3mttdvwwc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3aviiwnbc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3hhcmhouf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ufxbxjpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbirylms.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ivbrcspn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3docdxsky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjnluyjd.html


<!-- 参考信息 -->