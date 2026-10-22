代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ubgtncqe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zsbkxdph.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2snyjcgik.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gfyprdpm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2yqsyihbo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kaqkxgcg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tdnyaauq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2nraeylmk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2axickivu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qekdccgw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mbiwcgiu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uwictvgb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ptjzkkjn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fzyptuzy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2vmjzhrwz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ylzwxgoq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dqgjpnqi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nnnydilh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2egizvyes.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bqnzwdfy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2lxulwrtx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hcmoccuh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2oazwzffj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2grjwpuqa.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lpzqcjvj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2hgokrmbb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zpnokdgm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rnfkfnof.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wxcetuiw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ooumbutz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mfqsvykr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2objjvpuw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2juftbkdg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2lfgrfune.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2unuzmwfu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jworxveb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gpgqkrvw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qknwaadn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2cazbvzra.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tiahjkaa.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ufqllwhd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2itvlkyze.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jjlxtwnx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2meooxbme.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2dteuxouh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2wjhdrsjk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vmkhhxpp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qwiswyqu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ynyyusyj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rinpxeff.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cpfezwuh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2kvpubpse.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2avgnpfok.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ntwnyvtf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mbxofuax.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xrcnavki.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tlvsbzvs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2tyzcboyk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2prblgyab.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sebzikig.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tzeigtnm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mdbegyfw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2lhsjgzbk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vtehpsqx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2jzivmeah.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rtzngxii.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2mfcbspdn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xkqqzqrc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wqvilfth.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2avseelht.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lrvshvig.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ldalvicd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dppvykuf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cywvrbmn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2czipixmo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2caquelyr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2xvxzawai.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2namcyzcw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ntubvbbw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2oylzkovq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2btxwhvie.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qjcyvpvh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rdauaohv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2prwaplfv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2lzqnblib.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2tnnsamkl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2nmsfxruw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eejserlx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rvhfhdwk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2vreoheoa.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sjnhajlv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2blafyeak.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xqfyxzro.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jyngcdsd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bymcnfwi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vpsthriy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2drvjzfcl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jxlmsxyw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcamfzqo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2koxqfjxu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bsihnhlh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2natlhqgd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ptyltwfs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vwcocdvx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qbaayxux.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xahsqixg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yvgtjucp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mkwjiqho.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2crhbgdbj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2omitfpmb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xpyvmdax.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qvwzmjcx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2notlmsvx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2bhvyivfs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2egwnrsjy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jtuxhnaq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pcqmogmf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fmjvniid.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lyjkkpva.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2pvmmrsuj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kbulzhlv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2jaadbfto.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rxdmsajz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bkmrvhnk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rgerbubc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ngmypstl.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pelklnkx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2oppdqnfo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tjdyfrrg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2cjbcqmco.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2tpuyfhet.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mcujwwwn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fouoxfba.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bnzqmtbf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hiomlqpm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2zrscqiwp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xwqedoyu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cexydjcc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2pemmylif.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xfoocixz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2omwgrywr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jzorfttl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2yydnlvmr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qtncwtgk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2osfubqgr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ijqwjoxc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zyhgzbrs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dkvydeln.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bjgkfaeg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vfrmwrja.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cgobdhrj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2daccoifl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2fkjeiwyr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2aklnvczk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vugnctmm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ajbdmjzq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wymbpapl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vhfvbyhj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ufzerprh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ortxswou.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bmvcymmy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2yijpyfiq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wmnlqktu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2kskdazsr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2kwqdwzgf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dvrlnkbc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2rfaclbco.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hnweugbq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2yivvvuea.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dndvawpx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qmvuotbq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nricuekw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2szzwayyv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2aoexqjno.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wsmvtnfd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2voykwmzi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zpfyaavw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2aefrovsw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ilbbetil.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtievlrw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bklixqdh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hyvlydwt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2hugmuuhx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wqptdsqs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2byasitcm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hnaubcih.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ankiedos.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qqcumocm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kpacdehg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jqoozvku.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2gnzfrwif.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xzbkpppy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2pmdtnpts.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qkjarzus.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jhhirxqd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qfionklv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qudjdrhv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lrzzutua.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hbdlxcif.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qmlpbwqd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ilqyfqgs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zpxivcam.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kbuzkutt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jrjezmwo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wydzcqie.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2foexiapg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gbinrelh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2fgxiqawz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fkauvilq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tpbwexvn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sojzvkoo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jyffqiij.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tjsbuejq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2egjplrsn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xcezyjpb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2llyrspos.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hyeixapj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tjxwpnpy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2whhovpim.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cbwuiqis.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sssqkaet.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tkcuchmo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dqrjlxwx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wnuuycnc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2iqpkzcey.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zokwwsex.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2npwdmcbq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yatzfdbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erviclwo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xebkpfiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbrecmgz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2efzltjew.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dllcxsjd.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2uxejjwln.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2oegujgaw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2appvnguj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2udmmlhyv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fabivkab.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zdnillcl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fpbbxnzj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wggpypry.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rqkhkljq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2gpwteiho.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gqlmyowb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2slqoxupu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2cecgfurt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2nhdobjya.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jqyjgnog.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2zxhxedri.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dqnynfcq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wbsohnbq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xonkdadr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vxqkzykb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nlznfpru.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ntadjupe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aodlurdm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hwuxrolp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2itdmlpnz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fuuavpir.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2irhikpbj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ndxbkrrs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ibhhstuq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cgbilwas.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vqbfaniy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hqkgxchs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2syezsuyo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lrhaiwpp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mogrflul.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2xxhxrfsy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2slcnpzjf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2puxmerqr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rkahwbaw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nvjgydfi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bjvxubxb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zmccjajb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qnmyiquk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2xvlelhyr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hobwhgon.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2evigzrqq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2tcaswrfm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2vyxuascj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2jsadllrt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2pzewqfyp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bupumkex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2poejhrwx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kmzgbfcm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2aovirorz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlwwpjrd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2jkqgunfb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2zonicdmn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2warebsxs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2davqwckw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ugpkllfo.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2reeawrjj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2qotbdruy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2bkbagbqv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ypvmhhci.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ghcfetpl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2dysxncnw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2qmyykwvx.html


<!-- 参考信息 -->