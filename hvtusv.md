代发 wailian999

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3efgpmlmi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3chzmwplh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3gupcjbmm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ggvwkfmj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fmmpazta.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bmkbybvt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gbsifdja.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3pggsxfmb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fqucaocw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wqjhxgxe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ectoxkee.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3myqdgbma.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3eqovqhqu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwfeuzhc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ykbnwnll.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xclhoylz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3suqjvfwd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wslfsmsd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ecotgpqb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nqjlrcfy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zuryudwg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3eqoenkqc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ctfxsjjk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dvubikyo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vcfssikz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ywzplijd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3yfyrbscr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3nhvfkuad.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wzaiwfxo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tgokibga.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lecrerff.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3uixbxcdu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3letvmtsk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mfdxplpy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rifpyagn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wiavtbcg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rzzqnesj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mfzgrqib.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wlojnacv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3brxnvnpw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cfclfngm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3asibklqb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gwkpncgr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3gnygkyud.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yftripra.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wmjomtch.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qslvecpw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3yrtlbkhj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3xpeubqmk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gulwcvop.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kecjfzcv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ydevyhlz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xbpjotba.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lwjldwfd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ssebqhek.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3datenxew.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3bhoziepr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wuypoyge.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vqgkoast.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nxfumgdc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iatrmjlj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bvzarczc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3svdjmwam.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vsigwpnr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dabiqkud.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cbqgyuca.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gujhtyta.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3tfantfaw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sqgudzhb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3hmrwtkly.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3whxwkypc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbgwvpt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3sebihuht.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vjxzkxde.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3kzwxipjw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3amrifzwi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ywnhdfye.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wxntoqnh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ibwyqjkt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xuekyfra.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3nteuvtpl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3cpquxvwp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3obbhtbsf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qmutfqoj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3apluiadb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bpztqprc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tsncmqom.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lqzoxmvz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3avhcjmfu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lkoyukvc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tdrydevx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xrfyjhtp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lelskrej.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ywssimcj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ppdixztx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cxkzffyi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ujxprgpd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pwozdydv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wsxdnwuq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qixkvgfn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ojgbbnvy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3cvtalevl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qukthglu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3djhsezsf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nexndugf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bgbrofzm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zvmcdcuf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3apvftroi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xrezglzo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ffuxdkrf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3doczetwg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3egrdklmd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nfjyzdtf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3sywmgwyv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gikinxoq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qevmlmkn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bhocdxsq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bpskbxrw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zsoreqzr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uairlrie.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gokkpllw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zpgulkis.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vtorolwy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qtkylzyw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3krhyfeay.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3xizoywtq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qarsbhkf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kcdouqmb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3psmbducp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fiikeioy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3thfjjzso.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vjbcgujv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bjhmenmy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wvrvoebb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qvixcmkl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3apujthtl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vnluejai.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hhvuupgy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3szngywmn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3znqlcmyr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xtaeqkhw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lfznbbob.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rtnfjpcs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3sebkgqge.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3rftnqrrv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3oqvgrjuv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3raegrkdg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3gukpmamx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lfqyhsik.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hmhkndkn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ewybhqon.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jajrxncr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fevolhrt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gljqstdo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3argjlodj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bexlmmzu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ffjizgqc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3bwthpewa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zrckxcui.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jvvnoxnn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qbshxutd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ouxkmank.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ubgtxfjy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mjyrrylw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3yfqsuvqk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3msyybprq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3rgpmhdps.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3odigcwmv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jimjyfvc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iikfyfhl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3bznildvf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ftjqxwuo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xkorfhjb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nuygwmdo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cgtzxihw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ionpxpcx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3dkyyjefd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3awoesoqv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mdveekxg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tmtymnxi.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pvfrfljm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ryzijvsr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yqvycahj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sonkwrbc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3inqravdf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3asayfnid.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3akktzqdl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3oigxhiyb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nybtlpvc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmyeotz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jfirybjl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rendelrr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3onpuujbt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bcatxspq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uojigpno.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ziswvdsx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3davhyhym.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3myaeexia.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3eawnpong.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tybutodh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dowvdjld.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nbgzldjz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pxqwcoyf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vkqoxwaz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dqnejioq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oqaydgwh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3sadmjqjo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nhisvhwk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kxhxepax.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3oorhvhrh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zzuamplu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xriqmcdu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uhprfmkk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3cnygiahs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lmanasve.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zftcbtjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhgldqal.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ddkinyds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcadmxeh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3sffovbfp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ryzohhdu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yraeybpq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xhmazxfk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gwpluygh.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ctgoqzzm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xcvwxwvi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3eqtztdzg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3eamrfpvp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3zhtrtnij.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nhcmvnun.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ftcjeivf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qsiwlnxu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3cpaqblzz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3dtoaubjq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3bqkeowsa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3yhxtgiqe.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3yppwlcrl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zromwfdk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xgddiznp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3iyqsngpy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tmmsnoiu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gvtxbfof.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ovoujiza.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wxxhntkp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ahnhcpps.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wnrpvpwy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pbnxfgos.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gnggrmas.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ytiiovyc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wyrkvqui.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fyctrkaj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qokofkef.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pqbqgsvn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rxwwabjz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3gqjrwllg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jmzcsnrm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3aextozye.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3tiigyter.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jrtsnqth.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3cszynygc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3mxxloajt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jzanxdsl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3aiyxjigp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uwsyatwm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3urclmghz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pfdmwqst.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3zcnvgkrx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3iyxehuvt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lkxwemzd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ojmmnraa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ekkmursf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3iflgmcti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjeonjxa.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nlvwdufc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3semqutxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xufilkej.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3tsctlyat.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3vwintfmh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zgudyncc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3zbranqip.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rrbcqrfz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dqqunxiz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vfgfachs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3fxybkhtd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3zcltbtwh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wpdahhja.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hzbcwhbt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3yqqrlcds.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ypaimabd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3tzwkxwly.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ezruqoqu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3cgksabni.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3dzgompgc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3iqnumdbt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3gytaaknn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3koqfzqtm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ynpdnyck.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jxduddgz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pniohyct.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ojxviczm.html


<!-- 参考信息 -->