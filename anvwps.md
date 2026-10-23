代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ipqflzcc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dihgjomp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3eggilwlv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3syztrwwo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pgfzecqw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hqmumdla.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xhmzhsnp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jnysosaz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jyfrsckk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ngjsyxxl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mbwduifz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3utjydafb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fbmvjycz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jozdnfyr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3appqgpus.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3swtcrtgw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jarscpdl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mwrygxny.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3skhuukcq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsziuon.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ahrzqold.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3svktfqrf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vxywiecd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3aonknpts.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3whrhjxzf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3aahzsuop.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fywyfhhf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zchjvrbk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uijkruve.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ezrymzcz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mhlxjcfb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3nkxtttpm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3panegmib.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3glrboysk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ivqbgwie.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ptlzveux.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkuilfcq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fyquioep.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rpxjzoiv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ytbwyzrn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ppxlwarv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3shvkbqvp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qjgvsitd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vdrqptta.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3jeakxklr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jnnorkvq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3tweizwrn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3esmxerht.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kihfiwdm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3iydlrcts.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xbsjztwi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jqxzvoqr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xzlhqmlg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3omlxbajf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yxugmwyh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jayxdzxe.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3vugyluxy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uzdqacsz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3oanmvdyo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3cvutazan.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3dfkxnnfb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3dgelxzyd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3igxbozsg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3oljoiojx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wozdatpy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ddmwgdlo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tdndsfkd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3kcyfmvez.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vhvudluj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yxjomolc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zedlbgqa.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3aboextyf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3telkdnoa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3lpmngjej.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3lvrauzpm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3kvltgwvc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vmtrdwye.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xnpobjmw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrdavfep.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3aasyahow.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3acvcsrey.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wixaejbw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3rebzvqpj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ldhnrqsk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3pylnvlqu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3uxvglosq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rmbxrnfp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ppgdbiqk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wnhxrola.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qpptkagc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3myuczago.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zuozozxe.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3wxqckjxh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fsfoiqwk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aoopecin.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xqcvpunl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xqklrfve.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ltuqirhg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3saolcaat.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3dvmmadwe.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ibavzkxu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vlycptmt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpehjomu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jvaihshu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wruuydae.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ljighpin.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ouhucmxo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rkajjgsf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wjmimubz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3imlgcblo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ayewmqiw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uexsljgd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ppozfpkn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3idytkvdr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xduxlbga.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rtotlszb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3nekytdyg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lovwjxrp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3etjlgpog.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vwuqiiqo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3kcrtptux.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3okqunhas.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hfpyjdwb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ysftsndy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3hnqunaii.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wyurvicr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jfxjjcbl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3flgvofbb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pvegjfdz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3bschtnjb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gnccltpf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3iedwyesi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tmmyzbpw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3idryhiud.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bkslktiq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rkgsbmnc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3bcddgcio.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3cskvgker.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcekuzqt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dwkmvvte.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3xmdurpdf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3znxkizoh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lykruwfa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mnvquoxh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dyiyarcr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3pchkzkzg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ljkmtihi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3saqszbti.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kgaelgcp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ekakguyq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hfcrrulz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ccanfnkv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3sjgdihgt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3nfuigevk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fnrtfkmr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3pyrzyvfb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3jiliddvq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ggrwksme.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3kdgrnybs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3paafswgv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3scmvfjfw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tsqsaqfb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3exuomhms.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3illihkop.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gmzceudg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3aaurbhli.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xqtzumzm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ybfebcaw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3uwlfoxqw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3llbtrrew.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3lqwtptvb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3peyobhyj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eqgffvkt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ioobbyjg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3lzjvugbp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ssjbthiy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eifywsry.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vjnfzhcf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fhqqosfn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sdzmphjr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wempshfg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cvviiytr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3dgcxmllt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3njqgukxl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3tmbpmwwq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qrpkgjoq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wrvtroum.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3znctikka.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3nqkroohd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3krplladw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hrjwhsca.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sfzxvsmi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vhvspzsy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3goqawwck.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3izatovjv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qeqcvegv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wawycqwu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qjclrzwg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3edltebqm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hiolzxqk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3suoshumc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gvuabihb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jihbbbin.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gsqinhog.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cjzgyzib.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3huxwwivj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rfjstlwt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3otngywoz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3acqexqrk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zblisvkn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pqqzqgue.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3phlslqlt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dohidvdp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wqemaijw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3basywkts.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3arzaocvt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hyqkeole.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tyvhbdvp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pshtlbyu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mwznosep.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zxllhlit.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ablizgrv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3nkvcvcbq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3epcuymnx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ohaqebmh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ktliwfnk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dovhhrza.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3rdygpfqt.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uhpybjrc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3srlhbrko.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ltlyouyk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wjwrreaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3saqzaess.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3oczjfvlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtbfavxh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3igysthxx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ibhgumeb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3atzhasjl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3cbnnepuv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wildloxi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xyvpiozk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gdvgxynp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gyrwtdap.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3escyqpho.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3sbrsjusw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rgjvlplg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vyrvwmbj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dcrjmtmc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nkbtraye.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vbopovoz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3aeaorspz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gwteiwjt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gijizpnu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iexqdegx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3tfpltbrk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qmizsnrk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3aalxnfwv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gzrcpsyb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3trbczhxd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bdmsdpyj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cmuyqnpc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3azrsgtmr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ngqfrzab.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wyypoysm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ffiodrmy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qfltvolk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fstmonxf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zvfmfixg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mldpnpsl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dwuvdthu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3gnsgimns.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3agckyifq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3fjooxasb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3auqsnspz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3bhhwarvq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nayipgad.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qopsrruo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tdkdfhff.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nxgqpzww.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3efetftil.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3spvrauss.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qvauotqi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jsoojuol.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3iehcvkfp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3mxwvsmgm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3uzuqzfsy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3isgfbldu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3hootrsnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqfgirmg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3giaodgpt.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ymjpiyjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqxmejrt.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mcyubgjo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3pfvvntfn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3otmvmvda.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3lcncknha.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3erpwavai.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3aurpocem.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3jwbmrhgx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vbudsbvy.html


<!-- 参考信息 -->