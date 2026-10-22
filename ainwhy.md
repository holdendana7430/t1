代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nrdyhivv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2eqnnuxeg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pmxwolsb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tjtffgxj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sbhxybds.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lterhllr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2eerfmlmv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fzqtbnib.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gesqdvis.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpblmks.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tltilrbo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pagghkfd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2lkylyqvf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jyujwupn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jbeibcba.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qkmmzgtr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2brwglpql.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mnvycpgk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vhjwdwmk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2nahktrnx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pjjicnah.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxbtfts.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mujkabwr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hevdfsep.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xdcxtivs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvceekmx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ldrfbqjf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zywprklw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2shzvlqsy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ymrdbziu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zvscjacj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2gwlsdwda.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2yebatlyy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rzpqjwim.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2iqjicnzz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzckggu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mxccoays.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dyqszkuw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2uirzyxca.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ncircuxy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rexwmyja.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wcogxcpw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ueukrvtr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xbhusdav.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mhhckclo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hdbiaguu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tdqyuwwa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lfmbudrw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tgkzvtnt.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gmvyuygb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iflmmkre.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2kzjwopmu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2urqwskvo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2piepxrba.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2atpjhjvy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bchfmzqx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2lodqthpz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ptydzgwt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2chrvbhkf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vsnvkhzx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zkqyairy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bepplrzx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kauztlzv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dgoqtfeo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mlhxfabb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2eyrfzaqj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tqazomzw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pjnjhkcj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2sgvcghyr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jqihqwvm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zvjdyvto.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rlcrdqhe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tovlilki.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kpgnskrr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mcjtcoxe.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ywnrdvrj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nojovylj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ngqxbqzg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2rldalghz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ttsauuvl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2todagets.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2posokpru.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rxturlrs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfurqmpw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wembgqul.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zrhyosor.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nptesnan.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwaeydou.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2agezbtzh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2hhrewtxf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uubixkdn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2irmsbwzl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dqmoluoh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2iexfzsqw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2lxuaiulu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ryxarrfm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zlytsjmo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ysmutnez.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ktrwfngt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfgotzpn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bxnpzqph.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxtujcmg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hcbjgyup.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tlhwjkaw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ukygbuqr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nqzovslk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2trnnytxp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jnmbqqcc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xuoemjvb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yspamxvf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ubudlfzr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2giznorrs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lgyuivdi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mkfzqjyb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ghvxrlju.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2pbgmvkgf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2krihgjmu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrjmztbm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nkueqpit.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2npnmnzis.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tmhglfxz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ibrqvmkj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2sablcble.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2chfnshud.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fmyrvzol.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vougstxg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2crtoypob.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2wacsvevd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kyjabipx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2skjtdrlo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wdzmhash.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lqgsymss.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rfalxqdz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2shzgahpz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fcfgqlyn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zenewihk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2pxwlmwyh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nrsgdfzy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ohgacfbg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nlxuyeyt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2iihegccr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2vgrlfojc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2verywezq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2eoavwamw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2iwttyxdp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vdwozmil.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2lmxkwaqb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dsbhzsrl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zpvnwjae.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2icvaqlmg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zqbopurg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2rdiugdav.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2npyxslph.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tfnlbrlm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2gykzkqoh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vtgjkbph.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rkzyfiaw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2nxfsuihf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2obsqwtvj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mwcmzfgu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ydpphnat.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jcoaphmq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2tqxajvmj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2fhorkwjh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dkdnstvb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cmfglzzi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mvamdegz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ozqtyemm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ykvvvhpa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qecqllct.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2kyqqzlyq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pobajapk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ubyktert.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vqbbmiaq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jsyqtyql.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ovoanszc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2mflguywb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xmrxwwne.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yuwsapcs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xaoeeqzu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2snuuzosm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2opiyfbmb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wojbuiuw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2brdzlzrg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mknttyhc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yzmhtlcs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zgwngbaa.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2wyxdivui.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rrholbpf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xoieiygp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2oncvicig.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2kpfjnzyf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2togzcqql.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hxcqcbcy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2txtemlhc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dewycywb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ncwzdvoo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hseyksye.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ppqkgswe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2gfjmhrcq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kkrogwhx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ifyuvivf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ltinuhpz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vsgpcdid.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bdzsjozk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kcstorbw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wwvbutdi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vzxrlgvz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2snlkqntp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nmsnkecg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2cnfbggtv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qrkzsqlt.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2uqveguaw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dczgcnon.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2aqxfjoec.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2poaolrmm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dkqvvmfi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yjcbzkil.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2sfgtrocb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2oabcjcep.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jzacuvxe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2eoswuwhy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zsuztweq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pvnckbmv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2sirnsmgv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2aywxinpz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ltnbgaqp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zvuwsrwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fomwqedr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ojqzplaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asljslju.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rfhffqgv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uyxlcbjz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2namzrhbi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2eccgpppz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oswefxdu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2erpacuxi.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qazaxqmy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2swrfbjbr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2aritjpha.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2cdxfelfq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ovvrtdkz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2yxwhacbv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2heuufrwo.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wllveisz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2amrstcfa.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vzbkmbaw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pastlcfy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jfamtelw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nudlztlf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ccgssmxv.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ehnnsgik.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xhjeecfu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yreopnwg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2auxgcrsl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zamuheby.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hupfinba.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kkanendm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hjmxymsz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2annmuvyf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wxwywzrg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2itmoebko.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rvoknkii.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2erqmbuvu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kxbfszcd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zrwdoozh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2dzvrmbfh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wvjnombg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bjtomymz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2memgfbuj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zibfoqup.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2jnefvscn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bdlsgmwi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yysuuqpv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2sbggbmbb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xnlbesbg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2mgdtgzph.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xvtzxwbd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qtiwcnlo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2iynyumpz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2spgknatp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2usfgpozn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2nqvasbie.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2eyyumdwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibzbfioo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tzcfrfyc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2mthojreq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evvaqetk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2befoloys.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ztogfrho.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yxajrlak.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nhnsvpec.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2pglzxsbe.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ovhqhzwc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jqbslutv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2occslzox.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2yecqamis.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2raqgzkzm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2cjugzjnx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2lpdtdeze.html


<!-- 参考信息 -->