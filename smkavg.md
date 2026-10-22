代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2txfefjgy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2kqgzhnks.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qvdjeejd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gfckbhnj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2mdtcopmq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mlpimygr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rwfqudgr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2aubjntoh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2xxgzjkdv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qwjpheur.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2yvaoabjn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lhuyyylf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lanxxmdn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ulezkoai.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ghwvyqdv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vfpymdgj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bgoxzbvt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fohydybn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ffdfvzla.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zvhmlnvq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2upssrlyi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2nobwblss.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2eadgxkll.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dikynsyu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2makncoum.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2edrmafsg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2asafovyx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2uvobydxg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ycwobjde.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hzykadne.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kfznxehw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2svkwefir.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ghwognnu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2osjdycmb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qdypymxf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dirdbjur.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gdyummso.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2sqcdochx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ssghqrnw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ibfitinz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mngzbvzg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rbvlsrtx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bnmjaoty.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zqqkmnwe.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2edxbsjde.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2otiupzuy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fkkgtoqa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2yrdmcykh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2cnijnqhw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rpkxkzht.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2eoefnxid.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mcxduuec.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2uqmzrcae.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2bzqhrzyn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2snrunxzh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gygqdhao.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mfnzlvtj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ebixtvpm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jjnqweng.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2aziqrewd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dtaptpax.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ljffmzcw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kdpwghyu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2toeizazh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2dmatqmqu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rhkxspmi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2cgzcyomn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vempftnz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nigabomp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2osfnqehz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wmxptlhm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2pwjsqfgw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2fvmlkvky.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2scdauazc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uteqvpud.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2meivhjzz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2blfyzjhm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wvdxaoyj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ahptbolu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2bzramusb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vtsaevnj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vwvyubor.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2kqazmrcw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mlosqnct.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dgeyvkfx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bumnxrqz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mnrmmmwr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ymizepmu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2dmhashya.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2mnbsvley.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qnzfchwi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2aqznlfbu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2iosiabfy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2scxywhuc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uwkzsiya.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jtljmcgn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2wcalafst.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nkhtnjgh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lelgkapq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hsenkjpd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2eoranmjz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mfswkhbs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ltxsuhmx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2izbsjypo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2svrqqexv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mqmnvtox.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2znrkdsjd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dgregmdb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vlkcuxzq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nddipxlp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2usegqbrt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mqnfvkpk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gdarknka.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qansvkgx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2hdjpwiwf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ihietkqm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ibelhtcq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xinhraxv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2wpgwxsqg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2itvhwygc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ewsurpwn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ekoouekt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cospzgek.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2paeixebb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ugrzwhpm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hxgbvhbr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uorbtxug.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2aowmonxa.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2yodqqlzj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xbdyjqpe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ixkvkkpm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2omlgehrz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2qybqgjeu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2enevauvw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2owjfygnn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ffvuuzxu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vmuxbqik.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2aeckniee.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ujfeeyll.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nieendbf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2fowfvgli.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2pgqggbbj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2phlqjnvj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ogyxoxbm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2otlrdukh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2msipwbmh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2udnjwxpb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ilugmpgr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2znbjvgap.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2nvrpehak.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ounlawco.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xhzndgft.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2slfxpwpm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nvslfhhf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2gsdxzjkd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2sfolmnwc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qdufwhkw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2nkulajsc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zsqosaqt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2tikosjsk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zdsmtqjm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kfkbxvbi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2svfousdf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fofzcgev.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hvxdzetp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vxjtfyry.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tpgcbqxo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2czdqjhiq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2bawexcls.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2yzqdtzik.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2riamkahm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2abcaeiqe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dkqcoqtf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pkslpubk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2onlbchml.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vveuyyte.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2tzxaefjw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xenizxeg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2elxfdvtx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xrmmwead.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kpfgdxnr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2hmtdufqz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ibounppu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jxjieumh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2rlemytgg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2rtkjuhjt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2byxqndyx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fzaunjit.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2jgujcfqo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2putmqodf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2lxykxfup.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zakjzfny.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wqyfljbv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yncrlgff.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rktdigzv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ogacvakz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fbhujxif.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2csicwdau.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ylakxrwi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ifhjhqci.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rjnygmdo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ftevpnth.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mqxokuij.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fzltlvtf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dkladsqj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fnrgwtbt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2itxofaek.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2axhklfdt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2czuoszzs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2swswjbur.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2dljmrfaq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2nwvcuada.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2igsrjnfz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zwwkzees.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2blfydegf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2teugfesd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ywwcntwa.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ideunlke.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2iqdvmvib.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wdtvgdpx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mwhaogsr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vxpnaftf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2eotzekxj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2twodrgfv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2shmifrpz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xqfdnxea.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2klgbalfg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cnycfprg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wkpmytkz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fszdxhau.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ioslvgwk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xomyclaa.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wlsmdaby.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2jsjspxxk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ukuzxojz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2yocthipc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywxqgcdx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xjmbquzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sslvejrd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hzqyufwm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hsmqqiat.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2uhoecfxc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2kywpigrp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vulgevgp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uqjhgkwo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pxujgwnc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vqyeznya.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gulitred.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2usjyiqdv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jgbejrwe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2csmzhrud.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2neppiuhi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2igthslav.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rnxmragn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hgjdxlba.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hcqgoxna.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2xgtbivzj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ialajmap.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xfmkyxol.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2gjkttkpp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wpqyrvth.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2blclgenf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qwwjkitp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wmlstfyw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mfumigzz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dkklfgoo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kchefsfd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pijasvzk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xewkkwcf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kehtpfkq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fipkvahy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2justwlul.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aixmzcnx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kesgezyo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2urvuiwvi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zgedayyv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2lzqbgiez.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2wwpwavle.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2piepxhyl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2axjbmaxr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2aydbszlv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ckqwjlio.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2byazdxvk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lqsjjozx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ndeqpcol.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ddvshtcg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2wqwnnafn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zyrfzrau.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2fsbnccav.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2bpjdjmyk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2yillpcyh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bwsqsvvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2niorfexg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2dylxtyrk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wnsopcxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpuidmeo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2mctysttt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2mbjgfmmz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2eukmlyul.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xpxhgmro.html


<!-- 参考信息 -->