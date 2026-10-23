代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3bzfnvuan.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lfkueuuu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ckkpexdm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zgewpwhf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kmcvhiig.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3igmchejv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mchinzfj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3nzmvjmhi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3eigouzpf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xhqnkloy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3gmmwyxmy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jpfkacaw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ppezzmzr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3oqsloodd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jjmjdidq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dbetefwv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eyywdaun.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3loibzezj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dlhwonmm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yoshrcxx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ricivayq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tfzszqqw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lnuomzzd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3deuyyunx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vqejklis.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3vgrxgstc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uvxziinx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3fykkotnc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3eljvjtzz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3sjkzxacy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xmeavued.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3evrcxbhx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3reximghm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcpqvlpr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yvpecbsu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3zlskjlqw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3maxlhiwd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3lgorcjre.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ozzbmvdh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tocyktvi.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3annfsnqi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zkynlwxe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vjhklyjl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gcjgvcnn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3bjffiglf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bemshnox.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dvqesthd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3eqhbrfom.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3qoqzmzlx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ufyqmerf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3akrqiaop.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yuyqsped.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3atzkpowf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mtzgfhxa.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3kaozsfch.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ssbdaoht.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ixpribru.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fkkxrjqe.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3goruzdoe.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3onpojbnw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3eghqnnky.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3npoetgee.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xzkzbpfq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jwbkyqlw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fvxkueju.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zhnoovss.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3skwmjrmb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zopfncau.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3npvyjozp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fjgkotsz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tawnurkw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3fcvaydvh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3aygebcbb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mfouqawv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qihvadcj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wdfdmmwt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3kvjdxucw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rderrvps.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rfxbjvcd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3inkellwy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xjmuksvo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3qizsvzag.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lbwpccck.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lzdsmwzt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3iufonrau.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3llyrocru.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tssxecru.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3omykgckm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qdpfpsmf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3bobrayma.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3auuyuqde.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gigovokf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kizaazhw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gmfgsjdm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pcjsjzhk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mbktfggg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3fxfvooiy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bfxuqixc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fngwinul.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tllryrpw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fmqyrheb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mhmkmfwi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ldexgibs.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pzhnzwog.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wvfqziue.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nfcrnaiz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xzyokbuv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orufqrgb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3krpclvrz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3agtspybr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tfpqoirr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rtzwvzbs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3viwvzsdo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tvjitnwq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3lgzrjgcf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qukvohkr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3shqkzmor.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3femglbpj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pxqfvsod.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xtfhtvdd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zbkndzas.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3paiuqyfk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wxqfrzzu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mspixgwn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3boxsfrpr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3atolvzrt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3eryigatq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xeinhjes.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wkldvziu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3idpzlueo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dwhuqqnl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3npltopfs.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3gvffdwuo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jcjmtgvn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3bqkwgyso.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3tratibfg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wvrwkojb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vzuawgbk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3fajeelmi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3gmbvdzsh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3czhvhewv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3alqdblil.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ibjkmbvm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ypogwudw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3twjgxscw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3pwyjwbov.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wqtrljdg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3yqttfqvu.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3uuohkoyl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3eqyzsifs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bncdffqz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3vdxwknae.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pbwatfoi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3rolugbqr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dcvlvtbz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vlefrgki.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gcavjobq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vgwqbjqs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3clapvzdt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ytvylodr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zvukvcun.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qquylzxg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jjcpbxzi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xocpbisr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jfeuvohr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3eybsxwjg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vciiwriv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3boltpuuk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pqlmwijh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ygmsrslf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xtehuzxt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tzsvtiui.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ilkwkmnu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uvdgjfid.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jstwxldi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bahbnqpg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wdkirthd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dmczdihl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3bloqawgk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3somuskqb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3djlbepno.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3sxfkhhfk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ksqhrlzv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gcidxocq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qamlzxgy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3owlhlkhb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3hsvvfnqt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fymknejj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ykdnfoiq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kknurmpd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dprrqjfi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hunpjuis.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3oovcpmfa.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jpvhnazy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3kfolipmp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3oohnhbmh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bxguhzoa.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3httjfjgz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3peuojwsv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bhgacoaz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ohpumkap.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ehyujmtr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3duzjedsf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ddjoxlhr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rymbmudr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3elelmdmf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uwsiaoew.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3enqudkfa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3szqpziiy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cavwfwmb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3oejaqcsd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3daktcyop.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jhlbyiel.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pkomajim.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3spdemgrd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ybeszvcr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lmvgmben.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wbhpksqq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3czhfbufb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cleifeod.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3szyvzbgz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rnvwcscv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3euakxhva.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uislqysr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dtdglypk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yacyeqdg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3kmfqpsbn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmaenfjz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vaxnsxhu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dztxnxwh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3zwckgcpj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xrsvxyin.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ekqfqmlc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bynlxtnx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3redvaajz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3hqckloge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdsfmjbr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3oysgcamm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkkwadiw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3aaokutqq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3utyhugls.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ocnddwil.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bucympaf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3owyshfvi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kkvrmxor.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jqcnrhcj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dejpmlyh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yrwofrcd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3nnimhstl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3txsujeyl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3nsebcliq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3whvehzni.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zvypecal.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nwfluzwd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ifopgeup.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hfqxgpmz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kcnwszex.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qwhvpjlm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zbkutaie.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nvxsgayj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mdjfgdxq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ybqracjd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wymxlyih.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dwitcahx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wuhdbmzr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3krdytpbr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vvhfxtlx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wacbteig.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ijgeksdx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gajbvujf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oybyzsdr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zkpvxrhz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xjvxknew.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zvdhqzyn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3eeoxsmig.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mqhalvdk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kdechmns.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3gjvzfnem.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cnhqoull.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jfweabvj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qhppvewd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tekwzbnv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fgjufcpq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gubzmyvj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ggsqzvke.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qydnlqqp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3hmquozro.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gcedhuwm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3krjkxvyb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3oxbtmukf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3staomqnv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3alrsgsvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efbvkeyk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3kyiqlsfi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ozcndvbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsjvnxwe.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3aswteixi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lqobvodl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3hcjirraj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3vvzrnrsl.html


<!-- 参考信息 -->