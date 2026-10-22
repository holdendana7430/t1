代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qawnouvp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ewqrdfcm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dvhpvlmg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2getbhmhv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2wkzsflak.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2cscvbqzz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gnoiotpc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jiplxvdl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2iqcegbqy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xarhbgtc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2pyhoaxpo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wrrwojwv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uppldcyt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ipqefojb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ppeyfmyv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2oiwqmfxm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wfghxtjp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uzgstecm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nbernmek.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pulajxwo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tnbbxwos.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pkxuxjgz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vscshbhp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2iiawvpru.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2njkmscff.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2bhgyqkly.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ttrnsxin.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ctnxdiip.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nzbnfgkg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kcsouxof.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2jeauowho.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2siylxkst.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2exghmlua.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qedwsvuk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2armqmefx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pcnyvgxd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtirzdmd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ksbkovrk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2frowqpmg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2adqerbux.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xwlpodxg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2amyryudv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2gvycebrc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tmacgkok.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2chdpphkv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dpfqamyh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ofxarqix.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vtmwiqhf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zljzergo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ihusuhuo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ajlsxtvr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2esebqmbt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nuikypgh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2reqzucfi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2rgptmzzo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2scjbtcdu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zskpvaek.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2kwbxdbgg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2uvlncrxq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cqjbzcwo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ahexkzvh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jntsajfr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hzeczyuj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xkabhvoj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ikrtjwkj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2igjmxufa.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yhludrkw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kvuvyzpk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2egdodczs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2mwgcqitp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qtobfigp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2oxioxcqp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nfdspqin.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rebixafq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nimkavue.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rcciilrv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2amtpeqmr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ejyesgng.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzuunogb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2larrqduv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2inmcdjwx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wojgfddj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2yycvjkwu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2przgplqw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2kvvugjmn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ltqndtjo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lychlpcl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzvyumjo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qcopjxfg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2otuvsrxm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qeboynmg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ottufshf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ehchepzy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2bjeidkde.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2szbfimwt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2woclhzss.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2eltsjwiv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ggotajnt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ewhfieqd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2myxaufcz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2btuxyxwe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ulbpzzcq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pavhnzkp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wcuthqge.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2epryngtq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2xghiofen.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jkpjfhxz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2eatujdzp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qpgsjjdd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cjuhmqcn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vuaeoqjm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fxxmmnmj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lufdhgcs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gqbrtelf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qzepomef.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hgscfvii.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ntiemcqq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2oliybkgc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vhimlgru.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2seonkhjb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2mijjpuwd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2scdvfddl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vmmusgsk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2swnnhdrp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2boabjvji.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hhsyqlay.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xvetnmxk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vhmmsycd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2crbvvkvz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2yzkijgqh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rpullkme.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2csveayjd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mpsjjamr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jnqqtdta.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hwzmxxrj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jjsmqkgi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ejvlmfrs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ckoozjds.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ygcbexzt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rdyfecnz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wjxishbz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tvglcaeu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2lxtiuneb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ltshlmmc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2bsgswzjm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zipsvesc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2usxlnpmg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qxsvdnju.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zbwjlyhk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hezyejah.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ejwoyczv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wmvfadal.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2mytmdkwx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lvjaanim.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fsgwwnau.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2faiizfkk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rduzqwxh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2emloszpd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jpyviqpk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2iqevxwqv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2duhdpcwn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2bngpapth.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ysolhdiu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2nsjkdbxm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xvxepfmh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nwxbnzox.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2nkzyqvqw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2igcppixv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ecistlvr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ikbnmjpc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2uqcumjvf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sqtvzjmh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mfhsaixf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2sebikxzt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pftxtogc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ryylnmtm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wdnbjhgi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lhpxgliw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qcvakquu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xjgkgbup.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2owsztcmr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qocfjvqv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rdipjozm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybbzziwr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xwgkrofi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tkidztlw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2hdnybisf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2djudkcgl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2kzqkrgqt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2prppptvp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wzbqbeax.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2uaksouth.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cwbhnuju.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wsqfljwz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kgxovzyd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vhyalzkj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qcosvpot.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2douwlbbr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fqubyvif.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fupqquac.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mmqnuqfo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pfwpzzgr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2paiygils.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2evtzfazr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iezzybeb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zkbcowxz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2imxjldxs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2tfgcjwin.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xtctayft.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqglbyv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ecodjivk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2iutwuhjr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hqbfgpen.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iddqwwda.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ejphwfwd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ncpirnat.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dmxuhyjk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ktizobrh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xsldumnq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lbmzvpsg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ornlxejc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wdlhzbqb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hsijbunt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhftgsgx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2llrwpriu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jfknddmg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2plqrphsa.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2iebjghqk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bhenhbdc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2quiyaavq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mjqejuih.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ekxmfkqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opzlzhki.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bwdwkenu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eitbhntq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mwctjaxr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2debhrlqm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2zhlzpgzt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vofzhynx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2inxcrdax.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lbrxduka.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fzinsflp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pskjtjtw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2abzkldcj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2tbigfsqp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2enisrfmt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2evzbpinn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lmlaspea.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qdsospqi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2vksagawx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2uawjgfcm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2malezsyf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2blmggitk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2urfvzhln.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2usclhefv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xqghfmay.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xtitbkfa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wfvkzlgv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2binqjigm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qxunguyd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hkqvmtbq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2uhligxix.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fezqqiuk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pooiguox.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mlcvtqoc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qxgckutj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ljtbrgvd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yktuahxd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hxhhpzvw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2elallsdt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2xrrjizbz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ovzfqisx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2cjwpnhcj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2nlvaxazw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rxfpflls.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ajcvtezu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2sptprcsf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nobiahuo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cawwzwcs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2swkeawpa.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ytwcwtes.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bzaxcgnp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2dqxtsahi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ynbtdbwv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yhwkjyts.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ztyftvwn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nhqjxxkj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bqprmaxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btpuxxxy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2sbhymmcm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2gqnrbqep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2niiyvowh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ybewftce.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2sjrfxqva.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2wbcyiwde.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2sfkfflza.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2zybynyzf.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2hcjqiruo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2zbtnntrt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2kjzobwvw.html


<!-- 参考信息 -->