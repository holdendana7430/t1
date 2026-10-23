代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3uulfyukn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ctbbfbiu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ixzvmehy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3bghdydkg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3czuhgibh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hbscptdb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3vflrtgmw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3liwygmwe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bnwkekag.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kzkyvbsl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3khlugvch.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zohlrhzu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ixoinzpo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3htnfeper.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3tqesdmgc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3enrgoehz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dcuafcex.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3srtzhfin.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nulrojnd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yetrvuyw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mmwvbezc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zgknlqjl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vxmhxckp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lfzculcq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kvggxate.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3uikfxxss.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3inbxkygu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mfovnbiz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fgknowap.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ruplmzha.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ojsfuubj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wfetnjud.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3eiwvovph.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sttsrvmg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zungjhpc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dvbzocfa.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ynuhxtgi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3quwxocdc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dinmapxv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3myhorfnm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ifmfwsjx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ctwlscvb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kwionfvn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3iurgnxvr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yxbrwfyj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tajgmftu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3uyiqbkxx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3uggquljn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mqttqeyh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hebfapab.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3haucigit.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ncatrqmj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3qtdnichf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mkbglwaz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rgxvfgaj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vcoudzkv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3theokoen.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3hrcnrxhg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ppthfbsb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3efxymknu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wagpucuu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3pjmxhnfq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3spvxobhy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vydysccv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sycrhdmp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3sqgxshsb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zswkhjwu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ciorxtii.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3thewhnyv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3pmqmtkrd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qdgzddqy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwwzoutr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3waqgolmi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3sceeekiv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3algtnwxc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bbpezdis.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3huvuoxcm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3atgtybut.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zfixnbeq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zaipihxe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3gmmjetga.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjldxllb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qvtehdvw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xzdcjdlp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sxvljjrr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3beroalfu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wfcxlgqw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxfdjhps.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ypfiiqql.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mrspfyrp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nwystacp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uhohyrhc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wavsgeba.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ardhzgcg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qmhqkbyu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lbjatazr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3dyradkln.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mtnoazoi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3fsnyhncx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ndrmtxqe.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3tgswukcl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ymaiorhp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yuthqwpu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3erksctuq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3prvfirwm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3aeyunqsp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qbbznsfb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3esjobvth.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3uyadpffj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lmkvkqfw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yozlyior.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jvygsxgx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3nghxsoff.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gsiwchdo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ubgilpei.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bdccyaix.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3sjagfold.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3xgsobxau.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3cbmddwvt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ojptkjvv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3owpvxmuf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lzkvlieq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bxuyfoxk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3estcupqf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vokcrabj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ukprmaci.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lwcnmghr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rsfjtvpq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3wjcclpyn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3siqmptsi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wqdcqioq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rksixezl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xqbanplf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jvjccjqh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kvpewljg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jwtdmfeq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uszgflht.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3gbhypxff.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yuhmauyr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ebabtuod.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3atqimlfn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ktgtcrck.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3htafhrhh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3kdcfzzjt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cawfpyza.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3mktkvktm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ubdpcuti.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3gqqpmctl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3muvfzqay.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lshsjlfw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ffeqyvvz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3jdulmtks.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3pxifghxu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vvbsenpm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ujesbzlt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3diktowxm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3srxpjulv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qyowrler.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qbotpmhj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3swshqoqp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mpmdjtfr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3yifoujuo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3elsiygli.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wvuqkavg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3urrbsorq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wzvwxymp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3sbqjrsze.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3yrldpwuj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3uroozbmx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hwihrkjn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hrqejfsx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mbgslvbd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3trjmrryo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3snqjxutd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3apeeatpt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aenrmkwx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gybronyd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3xmqtitqn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kfhcmchx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kfxzxwaz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xaoeftom.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3kqmwhenz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ukzobaoi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kudetpfq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3pnahiotd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ngsakrkk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3msjwzlpf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3gnvdgxwf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3pwfglhas.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xuhhhmkr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3bnkdrjrp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3heodjjcw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zlddssys.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3twnvcpht.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fhfwzpak.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3iksnztrq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ylytiqsx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ekgjsqff.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xkebeean.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3auatrcew.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3jixmpokr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3irlxksnl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xsyjqzyk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rwbvsfzx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uhjxbuuk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zfmbudlr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3otfcabel.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3iwjnager.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rojafbkj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gcmnpttw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3lcgfwgra.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kbawtelp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3epfrmiit.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3semedbuv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3shqzyhfp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rfemvhlm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qpvpsnxp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mehywuqn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3dgtvuhdl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ouukgyix.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3torcvfjw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dcmukahz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xmdedhiu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aumnxhwv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cvfxyvhd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kfyzjulo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3siikmzmd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3uoqzzsrh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mlvxyidy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3adknrojc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dfjsoxso.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vaffnjiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rabbopdq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xquwzmar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uplknzlo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3nrasaumr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kxczjzey.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mptlclgv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xwhtzhok.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3cptxhbtv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3replpdgh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mmdgnfgf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qsicsnuu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mfwiysgb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3uuopsmpw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nmbogmim.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3hiexjnpa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3aehnaqdr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3oojkonmk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3izmwakfs.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gmrkfioa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3uvmkmzfa.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ahrmcdyg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rfiiqgud.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3knshdnyy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3hrzqjerz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kdlmvzpq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zcsxrewj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gzaiqvhr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kfmwuzxw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vkehreta.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tzmkevbh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ubnnyvoq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lfnoemcy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jpmvmkur.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qiatbxni.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lresvxzn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3amgjeiqc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zrxcqohn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ejcptbbq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hkdpoghk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qachllrc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3sofcsxop.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3nqwotkhv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3kyiaebvr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3uvhgegxd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3nxcluihk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jvqutreh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3twadtssc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lhvieljb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3jcwvyfyz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aihdzrfa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ydzmyinw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3risjpudm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3inrrvvvk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3knkevfck.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3blnukwbo.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3tylnilqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suydzped.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3wjwansqm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3uigjnvdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdmlmcdr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3pcqpcvhc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3zmyvzwts.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ezjqtise.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3yqvbbqfb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3xaplmnlc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3jgdkmstu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3wuvyrubp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3fljexmhi.html


<!-- 参考信息 -->