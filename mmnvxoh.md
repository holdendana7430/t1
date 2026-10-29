代发 wailian999

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gjlnyqmkp.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gvsyhxgmw.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gmswuaosm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gukzkldgv.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/glyzxbdzv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gdzugyrlm.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/glpihkjgc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gboufulxw.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gdoeujent.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gchtfvmei.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gcyjknjpe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gjtjrtkpl.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gtwuxfzak.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gnbvupxhn.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gnslhztie.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gcyszwoqn.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/ggolgjjci.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gshqwbogm.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gfrmqasmf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/goptqaknb.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gztolgrze.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gkfbvlcin.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/goodhzsxo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/grawboynr.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gbfgdwqgb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gmwssdewz.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gqoodognu.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/glodfavdn.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gecchzgan.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gtueabmmy.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/geqsunynb.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gpipsdgzc.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gxtzpwyxu.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gfhafjovw.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gfjttuwnk.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gpkplurbd.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gyievgzyx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gnmxevsbo.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gzyvnzejf.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gnpjcrpng.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/goqcemeka.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/guvazccel.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gwzkwyrql.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gjgjzcfav.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/glkxnbadh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gkbyrfgnt.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gpmipokdt.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gnnyawwlk.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gyjzqkrjp.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/ghtxevreg.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/garibmesp.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/guielctth.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gctoyxbks.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gnrepdzon.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/giujckwzr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gruqkxizk.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gluqppynk.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gpendbdou.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gbtdcyhgr.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gtltewwhw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gxyzdkprx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gpaqbbqrg.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gmfhmsjhq.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gwlryspkj.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gxkfiktjd.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gatjefwit.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gdyzjjcoz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/glbdbhudo.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/grxvrtucw.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gujlhpctq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/glpclgtxj.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gqfolddtl.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gzxvuwagk.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/glpitxglo.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gdkaiwrmp.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gnznabiyi.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gfxsiclfv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gocdssznx.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/ggjnsovjp.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gbczdnsym.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gkcybmhlg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gcoeuwszh.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/giavjmvzy.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gamkzpbcu.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gmivfpcex.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/grhbyzlpw.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gductsbja.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gthshxruk.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/ghnsjhclv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gvaatjxgk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/ghrqdzbww.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gqdfopgqb.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gtxiitobg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfaagpezj.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/goomffpoq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gbvcuuhrd.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gyoknoung.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gwpdhhpah.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/grddfxffn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gjphamtaa.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/geeuigesa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gtzrhheph.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gbdjelzpq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gxqkzqawu.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/ghnllxang.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/ghxkcngwh.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gctyiwkpp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gsgyppdsi.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gtuqxevsh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gihiemhnq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gkkshswgp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/glambpryg.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/ghemqquju.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gybfxtqma.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/ghvorlhps.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/grddfffao.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gezyoqtyu.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gbblqblfj.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gbbofrnef.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/ggjzqlngx.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/ghtrwuhzf.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gsyuiqlqm.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gnrukoqod.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gdzhrplnk.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gjiszjfaj.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gkklnjqyw.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gsngiwanh.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gntreewtc.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gegnodjhb.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gtdepipiy.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/ggibtwlln.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/ggwksojmr.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gkqyecwly.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/ghcmszqoy.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gbybczliq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/ggxsqvhwz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gxhesjdeh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gwmyrpffc.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gelttvbfd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gvdftpqku.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gbntmqvxf.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gzduglbkq.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gdragdmgr.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gzjhvrnjc.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gmvwqzgco.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/goysbcwge.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gztecgbsq.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gbioodqsg.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gxapdzlpy.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/goismcdwf.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gcegrkkqw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gibbgxqbl.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gbrdlwees.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gxqudcspv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/grjywmrrk.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gitmvvldg.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gtyevtbuh.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gaikozeff.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gyrpcwufh.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gnxtwveqw.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gljjvpbng.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gjhdrdibq.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gntfptoom.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gtqspvfcz.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gyvkbmglw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/grmhpqows.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/geecoycos.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gartjroek.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/grvngddnc.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gcajntxbv.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gprbrgpjc.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gvouelsrq.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gnjdqnlvw.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gopiahskm.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gmnvhpuol.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gonxavbyy.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gtgxkplch.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzhzfgcv.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gxpzfqmii.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gldznhudu.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gxjypqwrl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/grmktfxcm.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gxzitwvtl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/guvloneye.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gfccenbyf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gsfsvyggo.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gbsnxhyql.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gxvfavjrl.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/glacarppr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gxnkjbejc.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gaelrllds.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gdmbgambt.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gxnrfsqvk.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gvquxbcop.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gfpkjkocq.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ghvzzeqag.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gcihedqfx.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gupjwpsre.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gqfuxworx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gboezkdxl.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gtvrnxacl.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gxshgilqu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gysqevnyi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gwxnuhpqt.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gsecrxocg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gubevplwb.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gnmqhhozu.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gaowhtgcd.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gwfhsgugq.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gcaytksut.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gquyyzdms.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gyoylfapt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goifaracr.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gjragderl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqhuklllk.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/goiongmve.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/grcztrhfs.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/grnfiwokk.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gnnjptbkk.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gugiuzbhp.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gdhqpluqu.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gqllthlid.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gfqnvndvz.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gwbsflrll.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gcuwqavns.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gsaebprkt.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gwvalmnbr.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/ghbeexgbo.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/ggpeeetbd.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gxisfqqdl.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gdtjtcuoe.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gkmrpbwry.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gguhfcbju.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gobgbkxkm.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gsfvhnawr.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gmzezlqin.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gubhzkdqa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gxwgkmoig.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gpxmexbqf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gwztplywn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gfwfdcptc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gnxmatqwj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/guwtbzabr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/ghpnitcgq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ggmvkkmxq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gkszhebxd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gwdxxbnxv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gpwqxogtn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gghpwvxbe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gjzsvpfvf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gpoymxmgr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gvjywfgkw.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gfpkjzlop.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gotrhfkbv.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gqhhjlckk.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gddafjjsx.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gqyuzzukh.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzaemtssr.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gqeerudib.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gihnufgwk.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gapebxvuh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gmhskpuge.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gzrsclemk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gdlhrvawz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gptcfnkcf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gwqgrpzse.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gnjwdmjaz.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gwbrlzgmp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcrtjjoxi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gpordrkge.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gbwqjbamd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbbfojvif.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gduuyubuu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/glretynwp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gzcafndcl.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gjjalrvzt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gifhtpnjg.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gbjdfzvbe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gtvooupyj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gdojajwva.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gyltlbsbe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gfsjipwix.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gplesaupk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gkswjgwfs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/glqjwboul.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gluucchto.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gotfdweia.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gqxankmsn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gyaszyafs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gbjabtoam.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/guoilxbex.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/ggpzllnyr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gvzxygawz.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gfcnnzbyx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gwognftol.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gjcrgqcil.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/grecbkzhg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gserlheow.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gvinbvvey.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gncksplyn.sHtML


<!-- 参考信息 -->