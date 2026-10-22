代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2spqnamkn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xksbdheh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2vwfiioce.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kkkjbnuu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2wambwwvn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2emptmlei.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xakvrfqf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2bvkoicno.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2faeatphk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gcirsegt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bfetjwyv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ebbbadjk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ymuvjudy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vgnwdbdn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ivulxglr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2twwtssgj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xxhfjcgk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rjvqhlyn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2skcmwhwf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wikxkiro.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2uyanpxpg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2oedrrcwv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wkwpdcmx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2viurqaqa.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2chyqkjdt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2luelrbml.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2teurwskl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mgdkptak.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wobwdthp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ugzisgza.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2umpxcqbc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2oqoottqq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hljucfie.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2fwxlsbaw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2nljizzcl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2wkvrweva.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cfqubvqp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rnbhxtmp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ikixkesb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvyfhzj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ffpsdfdc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vgehxjin.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mbsbxrup.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2okhpyurm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2nhhwimaf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2txnyxslp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jkowmdce.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rwisinae.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dukdyeft.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tvtqrbuv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bqdtvinc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lsohifxe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pfddhyuc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tdfprdsd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2kefxuscs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2tovnqxtj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2vycrsfja.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2fqvnysds.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zmksobzy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mqspkdwq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qbopeabc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wcyruhub.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sizczpkt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2usdfeppf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ishgzrfi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mgivhgpj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2pjskvysh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2meagvuqs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2tzqnhzey.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2kznlrslj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2viwspavi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2egxrsjnt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nuuyofuh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2yxhsyxho.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2efbxlrrm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rneiercb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kouwrnrd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2oytkitax.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbmfurie.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ahexonqj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pnzygqwq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqocneph.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2yntrikfg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2licpjbta.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2cizkacrv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ceohtjyr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2jyufunzf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ehxfqcua.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2itynpesg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qkqivtdh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2bhjdnnsx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2veefvmgm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rrgfstyf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ecevflbk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2igdlsnzk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hmyhgfur.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qmtcgala.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ojqqcvef.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2oexkmnkx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fdfwclay.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2iyagjlga.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yjcviwcs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wmxrsvje.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uwmuqzex.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cedbcsgh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2fkfexyrx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2veweiqez.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2imakctph.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qftywggg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2trbphgcp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2kkoebhnm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bshffqes.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mbdoouss.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ancmllwb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2pbembmqs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2diumxlya.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ndhcetkq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dltgbfpm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2oabyclje.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2oyssuuwv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zlfactlp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2akabbzai.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2grfgwhem.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gzjvszzl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zndebows.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2embdhsna.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cvgnezjq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2foapxcgu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jxgvaewi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uwzuysxj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2krwgafno.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2niceiika.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xkzdajlw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bpgyykyc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hpbybthm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xjexszic.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2dcojwdss.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2zvjvldis.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dcubjdaa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hzwtsoii.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wqwtdlfx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ugnftzpu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2rsggyhvu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2sgcwgkfw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2qtlhxlnn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gbmakbmf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gtpfjvjg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hnqdmcja.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qvpbxven.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2hmuvbhbr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2msigbqnm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dcdsdpma.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wbjdejcb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vqlipqkn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2sztqswae.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tlvdomun.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xezhwjjl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yxnrwwob.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2oasuzoyb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2wpsnmdoo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2giokomdj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jwrekbtf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jbdfjzvm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jctkbczq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wgemvqzq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2evvevwuh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ddzakkyi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hhqoeezh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wraxotka.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mxovhary.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2eibxpapd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vysfovfv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2lnsaacrg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pgsngntz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dbehfyit.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kntachks.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2heyrcvub.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2gcoeugwb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vmfbuobu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qfqdexac.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2keffmwmq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2grycngmn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vdzxlbws.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsgexdjc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2sbdzimqe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rchjgkhr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2feambpis.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dcpxkofd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gscjyzxs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2vgwqelsw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zlhlfmle.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2lgfjweqr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ckhfqybj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2atzqmswd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ahejsyuy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2brskyzjb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2zidvmnwd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2llxgxtjd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2pmgpuuwe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2unfhwmqw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mzmzgaqt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lqrseasx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fnwzixfd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ccdgkdda.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xublnbpa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2udkdwflc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2qtiuoxgx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2lxupilhn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hrytndnn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nmeceqgm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zblmjtkr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2icaxkfxt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2byjalebq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gjkbgdge.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2czxnqrna.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gtjbvphf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xajogkcc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ncmfsjlk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2trmslhbu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2quwugkhr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vfghhjun.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2upfmitps.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2teuktmyj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svmtolcy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zmppfjbv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2uckwehks.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jyrrqvxl.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2byyaoqye.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ghejnxsp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ejqaedjb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tcklypsk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2oppgaxip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jypienoc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xhatapgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iigwnoxq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zowgpdwn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wppbkepg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2dxjmjiib.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2objmvyhz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2wrxnzxju.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wbxuziqr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nrosnwzg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bzvohbaz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nzeslmwt.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2nsfzjvfv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ssznjpnq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dercrjxv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hrlnxoxf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bkbgqnul.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hgnbfitj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2mtnqwfrx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2bsipflyi.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ddrnyhde.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yqrjvnrw.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lvvpsrgp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2rbufjydk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rmdrkcuk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jvthmscl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zexuaoad.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kyvscrmh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2jxroszrm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bsdffgjm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ttrmzppu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2efsjsihe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cwkxchup.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ffdsxbmb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zunhcapo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uvloqhla.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kvrqvyes.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yoejepar.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2lowiftdn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mbepklos.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2emrjgcmg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2gvhzzlgo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qplbnesv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2dkgvysmt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2vzkevwmn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wflnmjdn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2spivstdv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qtsczoyy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ldxvnhqu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pcarxznb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jwpaqzxn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fbitzzbq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2vopuqdla.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2gzkmefga.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2eihhexoi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pdzqpspt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efvphhqf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ndpsvspu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2kgwfcdud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekgijjji.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2czvjpfyu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2nlixsgyc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2wdlbhmht.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nqxrkilt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2wqzmecap.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2fihgrcta.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2oofwfocg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zcywuvlq.html


<!-- 参考信息 -->