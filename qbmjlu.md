代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2awonqyrq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sotdvaab.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2azuvbetp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2hdjqkfie.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2aauafuhl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vsfwzcax.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tldypwsp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dwfakmlt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jdivmlnb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qefiverf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xxklmgwy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jgwsatfn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wfxlykzh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2getqtptw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2fdmectbw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rvkdtlfc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2nystlagl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tilrsdqg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rfqtdjai.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfblysf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jghstrff.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rxjdomqi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2iymrvsna.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yqhpsreh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qrutagau.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xxefofvf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2iynaicqe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nvsiiprv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zxsdbvtl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2efxfggkb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2shxibshl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mxwovuuo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ujewtzne.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gewohzrc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hzkebjrj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pjyjuiey.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2wdebebcc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2auqywtih.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wyutovqa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pwwvwttu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2nrpetjrj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2jdhtdzxs.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wqrlkjzb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pnpsdqnz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ztuwpevz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mavjgsnt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kzddiidb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jaerefhl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2uoqmjinl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cziwsliu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xbeezhgq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2mzwleswq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2vhtmgwtq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fvypdvgd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tpbuzxfg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zndenbur.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nocifewk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rekaeexq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xssvbyzh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2lokjqrvu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ucofiphv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zzkiqnlf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ndctznhq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2aylqnkmm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wjljrdbv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2bligscvq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cyogzvjl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2riwlyfpl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2luyxpvvj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rsinkohg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uvhhppes.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kpdibcfu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dutgwpbw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ssbxexrp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2gobbqetl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zxwwdffh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2kfzydifz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2yqmmwfys.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2nfrrmnwx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2honpbgaa.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2padculln.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cveuzaqn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2zoubxvyt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2gydlgecu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2zpioglpl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2yvosupkc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2goqmtsfr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2iiybgtxd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2rdqdazce.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2adiycjxg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fpqrnfxj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2syeakkzi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fwqlzlbv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2eewrtrkz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mhfxzvpk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wagmljxn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2mrcepyys.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qnlbujzu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2sldwyjes.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2irszgycl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2utriywpc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2amvasuip.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vhwjdocr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2opxfrajb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gmhqccth.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ruejsfnb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ogpczuur.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2kieukqce.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tilzkywa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pspusjiv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2cmmqlrew.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2nkjhuarl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2aztmafjm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhcvyqzl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2mpgghdnx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2bwtdbwnn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lvlpswsh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lwwirznw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vrhnptsk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vvgcnlro.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2mpretrpo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iejmnfnj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2gblzmhxe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ndczyrof.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wnmppaem.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hdlizxum.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ecksjkwk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vxeymhyq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2yqjnflck.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mnzhuahw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vqhistzi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vrsfvkqc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2piefwonq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wuiiweid.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rhjhbzzo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nlfmkzee.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vdsnjqfw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ilxlrwvn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bjaidwax.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qdkanult.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2eqmptuye.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nbthehtz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fuoesphq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mrnomnwm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2fqdobgkm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ywseyhim.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lzqztbqt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pohcumfj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jvejkqfu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rnjeydvk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2kkcpjxqf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2cpmlfqju.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nurshtgl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vsshtmej.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2bwrjxmjm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2hedpvhos.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jjxerokd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2amuvldhl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2dhxyepjw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wyjfgxvc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2bhidpwld.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2kzmgxqbn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ypmmvotz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2cqocfsuo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vuiwvpfz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qenkcnxc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kpwhghfn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xxruymwq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mlrclgss.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2atygcgol.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2oyeubuvs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ufgbpmqg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kirybmlc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jiduiztl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vlrzstzw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2alemyjcx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aemgrjdx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2bfbwmjax.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gstnjhia.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xzlwtcuc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tezjhegl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uhemciea.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qtbjqzdo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gykhwlep.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2egdfzimg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zzmvxbnx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ogekmzai.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ougjxyyp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2trhrddvl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2goufmksi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2irzvvczi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jyfnmrvu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bxndivxm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fdpluscx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kutsxnjc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rcnsuagf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ylrwnygk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dcmuvzju.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nfykwrlu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2crqlunrj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vhovirye.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lbfhlcqm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tvatajjf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2aakkscwr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ioyjuvgw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hryrylxo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2bvpetwmt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dxwiyeke.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2maixpxmc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xiublznu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gcgnvuzq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2sndderfz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2jublxgwm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gmkjagxx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2yrmstmzj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fwufijnn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2pmgucmld.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zrgeilcg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2axzzlide.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gxlgiigj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gqazeeaj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ldgxkapd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2tnbvwcry.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyhriupw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kjrgzlrw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2dvsryqfq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ciimjbfp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zairtrrv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2wbxznjkn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2cwpzicvt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2oykpicdg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2bvldlyzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qoqdalot.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2sjadvjkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcijyrnz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2rhpihfaa.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vqgdwujm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2frzmnitq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xyoexjnt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jfngjvxe.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nirrnuku.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yqlkmtxh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vsqcbpmy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2aaoddyxi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2lbzjoeot.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2kjltuyli.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nuuuutnj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lphrplnw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tkwlrpgv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wzpzpadp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vtemdjpr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ueagzncq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xvgsxgmh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wsnvenph.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vepzpyvy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2uwphbnup.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zyybfdzl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ejfhjbtl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nwinbxhy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yxyblphs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2kgickfrw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2eufbhgsc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pcpikgvy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2bjnnijwt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ekntdper.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ropahsgy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hfbvffwj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2usjydicn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2stwpitxv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nlwieabd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bpplgpbd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ybbcnnen.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2raodzjdy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2qqnjrnws.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2cjwbvgem.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2iaovaqto.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2jrmnpepn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qktxrlka.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2hwsychtr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hzvljvku.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ybdmkkst.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hgzojpkg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2rpwwvfcq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2jhestduh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rwywaikp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ovtjdgbj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ukdiakaf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bvnksgur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcyqktff.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2fqnjoart.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2eqdwvjfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcmhwoye.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2yjkxguga.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2iqthryte.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2zsfxrzvr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ssbxvczt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hvqfbxch.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2moylqree.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2enyvvqla.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pxryabqk.html


<!-- 参考信息 -->