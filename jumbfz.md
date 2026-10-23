代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ekzzqcco.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3oazqtycr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3aqvxszvm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3opjdbbxi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mectwmvd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cgcnlars.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pnvibkft.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wsnkxbaq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hfexqoys.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3kgrtnhuo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jueqixhr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ubzxhlki.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rtutxloj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gajvkwyj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xcirqgzx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cmmvfghh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ragcxqer.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ukjebnok.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3oryaiteq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bngtwnju.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3koivnlfr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3enzhotpn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3lnrhucom.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cdrsfnyt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ivlkkexv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3crkuvaew.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xxtbwfrk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wegrkdym.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zfjypltl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qrrdyrzs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qgrmglnk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ckykrsnp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vacqswzy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3nabzqyec.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hzryzckl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3eiutakpn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mlzmyqyt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3frwqioku.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3oxfgkmuq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3qdvvrhsa.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zgxshxfi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qzpyiqwy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ihnyqojh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3smbzpwmi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fcceoaxb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ffjdvcbv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dwbiekoh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3vfjpihsf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ymororam.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3whowollx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3bcnfsqgu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3cnozrtkx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kcnuvmbw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pahitwss.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hgaglwsk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kvisazqc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nlinyptz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jronsvua.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yjcpiycq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3axtsnixj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xjzfuwah.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lisozwct.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ttdsneen.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dxlrorvf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3csejsjvj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3oaxdivnb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bcxkcqeg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vofntntc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wvkfdycz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3untfeubi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ykgwqdzg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xlnpxxff.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ooesppxz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ynzrffzi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3klwqqbnf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rswxqlzx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ejjdagsh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3btimfpae.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mzodwvhw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3atxqdein.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3imubavob.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mljyxusn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3olnwexze.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3aoriojbx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3jlwrgixg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmhhteas.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3yybbmnsn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3zmkccimx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xziazflm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3fidumyzr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dgyxvzzd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbkjhtgw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ahtuomhc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ppbxmqtl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3sjxnwzqv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlwtzswv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3slcsrmxr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3icmupvkv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pbbmmbjv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hvebbfis.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qihfzicv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3vufwyuwb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3axmsxscb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ijzwquxb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hcpdebdh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zbudvzbn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ejjrtnrs.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ywybzmsj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tnlaheau.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3isnbsnpt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zpxvhcru.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ulwiloqi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ycrupumn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qkhptbwz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ffqostck.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mhywopih.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3medcyibm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ksatfmbj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3rssnbhfm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xiwhscuk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xwrmsmqn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3frgxybuo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rqunryvy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3iojtznjb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3yquxvwlt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bfqyrstb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gowfjwtd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ptfckmus.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mzwpbypt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3odffoipt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3citwotny.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3aeypikxo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ihomdpjv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zcrcypyh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3juudwayt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3burxtyxq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3netyzsxp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3lxmfzusr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3lkcthclw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3tgnrlonk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zvebkhso.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ecqinepk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3blhghgvv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ggoxtwue.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qsqyuhyq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zhhnmrpd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fdnliolh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3cyjwzaew.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cmntbyml.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3cqthktkl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eqyggqyt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3yyrczehb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3izpapitu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3adslszrc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tjwxmcxh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rwprkyen.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3pvkaydni.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zmokdmfq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ctmtletk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dmpvpbvl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3fcqfjain.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3syxtkdif.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gaqyhjvd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3fvggggif.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3eplgmizv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ggaanihy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xxkcnknq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3nxtoqnwi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zpvjwsas.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ggumnrgf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zwhsqouo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jhazpgog.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3cuevbxjp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jclmgkuc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3brimssov.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ilnzmrow.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3olsazpnx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3voccvszo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gfwkdkdo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ybpfeeik.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3trcvvoqy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hupwzomq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dytutsru.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qdxunetx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3jbxwzuob.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bayqoyzu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qwgnucul.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wktsltfz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xzmnepvc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3alaiqqdj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3btafogpz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3zgbwqpkh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wnmxqpgb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ldunbwqz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3msurzjhx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3uurjrdyw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3idrggdbf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3zchhxrpy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jprwxxlj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3pgwqtbre.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3zedvwvsk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3frvumcye.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3swsbxwhf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qcpiirza.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jfqtcsvv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ylslaper.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fvqktdeo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ffzxgneu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fnybzedi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bbmsdqmq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wgfoanqt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fuwauboq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vkjiyljq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3juqmdzyt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bszqecnj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xsasfkrm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uzflxhit.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ddtkjdpk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ziewdzqh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ecmfnbsk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lmotlfvg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hynojctg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3itptyhpi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lmlvnwlk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pgxraqkk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pmumqabo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3edyadewm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdwxhveo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qhzysauk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jqxwnmtd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3wofvmimc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xgrrbdum.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fhacqvxs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yeknppsn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3sqjqotos.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3amuptosd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dftotlov.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3kpwijqeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdlscdhy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3jwupbidx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hswimesn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3cjvbdzpt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xxjdqykm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xkmrbiyo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ahkcyakf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lsuvddyd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sknednlt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3icwieate.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rfkqnlsg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zjeqgnpm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3klvlejdg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3homznpsp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mwhfuimv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jtovjtcn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nanzfxmd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jenqwnfh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nbjtnvtn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3njkhgzed.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3aedexiib.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nqqkubpo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3stlqevig.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jaagokya.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zsxgyhpg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qoqljmcm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3wdgmmyjm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fqqbqiik.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cocwngeh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xuemikur.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hsivzjce.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3clslsiwl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jbznshom.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cvohrfmr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hqzlhfae.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bcdqhnxb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3oguioaqy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cifcktcr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3eytbeiub.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3tbubqfun.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3omwxbgpd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ssfrwvbp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3prhhhmuj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ougeaocc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3glcfuqia.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bnjayahy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3mnbcomto.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ndgiagvn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3cotymtyt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3iwjzdvfo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vgjmpllz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qxcrmvfl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3xhffbkvm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3liypabro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avjhinqh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ctscetmk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zynszlhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mocxdsub.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3satoxflo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cgrvjrcf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3picqnhwq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3asbujzpa.html


<!-- 参考信息 -->