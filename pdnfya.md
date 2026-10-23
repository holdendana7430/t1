代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xcomwljx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fqoftxjf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fqkiaoyw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cnbxqbri.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3djvpnhsf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mfiueuve.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3sdrqadah.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3gfuurtah.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vxgyhkja.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pdgumnsa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3iaedsggw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rjyquuom.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3oxcclqmw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hncyemgz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3srgarckq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3sdlvushf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dbnnvprh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3riwadpqr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ajzchgtk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eulptbjk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vgutgkbl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xrbezlru.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hwhjkhfw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hjrripjn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ljrfkedm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jmowtqbc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qrcvahnc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lbdtvlcr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ediexorr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qxyqncqp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3iryvxbat.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3znolxxbp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kfoyxllt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjrnhigi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nqbxxihx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3focvsdpx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yhfiufpd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nfgsmxln.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xwilazvk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wevqdowi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3lhaxvijb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jyzgjxqa.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3igmvpayq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cgfkwwow.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lkrmajmn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bfldtsht.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3okjrnswh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3uuzqdhlv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ieanflbo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3raqhjyjq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3boctkhax.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vunhugjn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3coppyjqs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xcrslglb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yfqpwzrl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3yvkiwcvw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zzkvarmp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xweziicd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3soieidnh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dekdccpv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fymqzdfm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3xnrhrfui.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nyyzhhek.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xtpeyxtz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3augfifnk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3lykafqop.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iaialofk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rwspfxwj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3eqxxzlkg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ftlbyxun.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hfrazugq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vjdlvjxs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qoceseuq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yddplfqq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3lgxblwgu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqafelb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3arstktsk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xtrucbde.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3donexrai.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zhlvyafv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ocpvhhzj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3gtjlamkt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3rqcolcdk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ujotqvrd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ylyqlslv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sjgznqyj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmvcejki.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ynmxtqij.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3aoghxdfj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cjxusvos.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zhmvcgks.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xejbpvvl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rjaudgsc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3uawqfewf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3cyhxxied.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uokjzyez.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wqgsisyd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dizpmctm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mdvrpjqp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rlexhtdv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hakpputx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3jolpgmoy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rwwhusdr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gyfdthrh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fznwyoyc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nqpdbcbv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xvrpqmtt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxhgaguo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qhwviqwg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3rkyntrrw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fughawnv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3efjqhjdm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fmexyqop.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pxrupahq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3zgvfdkug.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3namcixgj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bzqqzglq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xwaazisl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ctstmqga.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3avfhwvzn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gwobihuu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3yoasdjwp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kihaxnue.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3dwaagryo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3cvfauoae.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3grllghyc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3daetvhne.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jdlhqvdv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3acgbxmxw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ualhwlbm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3sjvquwdl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rfykrcpo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jjoastmn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3gnbdbfrr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ccvfhbnr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3gzeksiie.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qprgjbuz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gmgbtcwh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3fcjyetgj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3inphfnrw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ssjbpgee.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3yxrketty.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yqnrjnnd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bllzrgjf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ezbzoseh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cxgyupuz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3wvwdinzt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mjifmmzd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bfzcexpa.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jwesglse.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vkuvwsyf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3elglqzzu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dcorbrjv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wxwqfctx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3jnwpefhp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ktqjhpcp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fspbcfup.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3kjrxtrap.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tafyfgty.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3utxiceyx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ijshdrce.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qzpupybj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mhtsnscb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3oxiblqaf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3blenvzdq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fngzhrnn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3opqlhhja.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3glwxtuik.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ulujalyn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3amthdlpo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3lshywwuy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3krsugywa.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xfceqong.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zciqkxzj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3dyndwtis.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3djohfjok.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3phufocdl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mqfsicym.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3kqhorxsy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kkumlpcj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3fjvnlyzd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3juggroon.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gzqfietb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ujwtjfoo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ylgfnyrt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3aickngom.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bimsrlfn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zmzeqcin.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ggqddxyr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vmemsyrd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wkeoobro.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3evokvdrp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mcrwnxyn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fukcbgun.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tobjmpmz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3iihqccqa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3alkztdnx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3frsupjqd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dtesqinx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hdbvgrtk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ktuoimvz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pflesnlq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ppnycuxr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fkgaplwg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ccjzntkc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ugbnsvec.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3feamvjnm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wjpjfqjn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ihycbvde.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3aogazssj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3poaonsgf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ukpnmhrl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3impnisjb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zasbjdzq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3woebqdoz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ipfeawyw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3drztmfbv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3aqivjrmb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3dagrbmhx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wddyryxh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3upftwqga.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nrfikscj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kuymqntm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mgqkrhdy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nucvcarc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3batqhrxd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3cueiybxc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fdoqeyvc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wutlkljx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bkketwoo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3psnplkzu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qxqppste.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ixzbeabq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qbzdsfse.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qqwwbaiy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qnlmjorz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utcextxx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3rozeksyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbasavco.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3sozjboyz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jwnqprms.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mrljgpfe.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ofqjodfx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yvtvxpha.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dnzknllk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rlazlwng.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lkuuvtog.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3guxncvpo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hstjogjt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3tpkxwdxp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3voaligjc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3qofelayb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rvkxvlfv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jkxiqumt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ecpifhqq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yhtudhru.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tqvefbtq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iwyjupmr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3awbjyypr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jfnzzmjk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3cazebiyn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ilpwqoqq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oeijrkdr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3smtlprvc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3lokxnnlh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mevifjnw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mhcvebrf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3epaskqre.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hbllhntr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xmxnndhh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yihkwnbl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3htdzmphd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mqcsvzgj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bxmivmvg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3lrzcybeb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qkqtrdwc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3hjilzrpi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ngnsdims.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pfhhtqil.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rnujlwbo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3foqkhtnm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3umoroxjd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wqronymr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xxtpwrih.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3pjvvoigi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fwzyahhs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hhdvuzal.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ecompoll.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3qgjuwpen.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3isgmtgwb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jpyrrxzc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3hadnsjgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvglbjgy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ulcrfrmq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3azhwdhyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdxppsup.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3cgsvgrie.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3xwsjjoir.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3gorybtxm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3swcxvtjj.html


<!-- 参考信息 -->