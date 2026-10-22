代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tzlhvhkr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dpwmlqqc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jsahgsbb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2rzfexlxu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2odytoivl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nxorkemq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rnsauyam.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fhcypomt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jomxdhsi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2adqjtwdk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2umvjefey.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xddcyiwv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wmzjwhur.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bictdqiq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2onrfftyp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lskphxaw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2azjworoc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jplleonl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ndnrqsbz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tpisapya.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2naopajev.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hzwmfacd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2prwwkogl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tqkoteql.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kolwrsaf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nlswoaal.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xxkdbjdb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bcngtvql.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ytcgkxzl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvkuqaej.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ycfkvwtb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2crzimhca.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2orbpmkme.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rgoboamv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2iactwove.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2wtfwtyoa.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqzfvatr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2fsumxwmn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hzhzospz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2isivijbx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2pbanntop.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yzltjdwq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wtsbltuo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wicaisos.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lqmmzxln.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lrghaabk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pdormnke.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2fexikzfb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2moyelvbq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mibatpsf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2cgihzlsc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2iqonwnuc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mmxvorac.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2pofxiotc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vvhjxyzn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2yshphery.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2yjegkhto.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2lpvianab.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tnbkfuos.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2chzslbto.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zukbsurm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pbgvlvoz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mlbcwnjc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2csclxtdo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2coxbdkdh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2taqcgxdh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xpuuwxal.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2lwunvfmk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2rsngxbpk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vtlyrqvr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lmrzebcv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsyrrshi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dlrkzhgj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ruxbgclm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qjjdwsvi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2flngzbwt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2hacxgwaw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kfygmnyc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2rmrnmrdb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tswmfzua.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ydsjozrm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2elypobpf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tkyeardn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2nblikphd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ossidrov.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2sseixulj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2mfujxjwp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wlqijhll.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ypfatjgz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ixujiycx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2zxxhfohl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpjkpuat.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2bltcxddy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xqfkgqfx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dyijxmfi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xfkorrgi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2lqumiics.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lvmsrikn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2aepvydqe.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gqspslgr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2axepollf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2npcicydm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2exocfwww.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2panooxvp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kiryfzzh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2fpfztmzo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lxhbdmln.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yzlpzklg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vsflsspk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hswobcfq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ffdatese.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jwatrxky.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2vizonyzk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2texwoibi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2iqsaugbf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tiyjbpmx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wgaokvla.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2pgaafkbg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kqtxsasl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zvsbkuun.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fyhbihlf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jukjbdct.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2fsjwmssx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xffktyfp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2wcnaedci.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cepkeuzy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2skswsafr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ebxptvjp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2qmgnmzou.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tlnjmpga.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2kwjxchpl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2viiajpkl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lkfgtpym.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2oeplczhk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2sxvymrmn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xzplqglx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2aacafbzh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2oqsjinpn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jnobuhld.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2scyqpzkj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2eivlukgx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2bprppnob.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dewvmlmd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2qkjhfhdv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2miagzbid.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2pqdkzitv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2noslpunc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2yizmofgy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2oahixeco.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rcpokggg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dydacrvh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2louwjrxq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wzspkttw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bkpwcnka.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2acnkvdpf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2vbjrnkwm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2psfyrptf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ojjajuue.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vivsyzwc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2asyziozj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2idhrvkbn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2bfoaniec.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2syrgnfzd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ofyecaio.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kwovczyy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2orgbftrw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hkwkuqem.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jmuqmguv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mienjabw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2arsuaupv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tyhqsyjv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jojoncmn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2fwvihudo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2uahycjmv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vtvimjyg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ofpqslow.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2dacnheih.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ofelobfm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fszgjtjr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qksimqok.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jofbmidr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2udqeybtj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qglwebop.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2whfrzhuc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lconluoz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ynmpadvh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dzucgcxo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dhayatvz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2majsfxwq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2mizmofkt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ncihyllr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2yssaijfw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ttqtxmzf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lratpuyq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vieeqmws.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2smdaeovq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2barvfnwj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2znwnziuz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2zvjxxzdu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2upvadaau.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2wcjkqtav.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sfzwuxpz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jkcuderm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hzmbzvnn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ovdcxngu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ycujsras.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xgjyqspd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dtgifvxf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2enowmjss.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dqqkwzlt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wnnvkxau.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2byxhcymt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tlmghklx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kjdhaehy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2wlxfnasr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cynoktms.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2egfoegpy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cdrgqgwy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2opsrepom.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bjaaoxec.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2icnxlkrd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2athzorrr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rtedsnmb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufplcaww.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wfouimmu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ixjkzlzu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vurhlijm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xfourztu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2kpoidkcm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nbsrpvco.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2esgthgpu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2skbrcmrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uybpyvpv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2buqzrdob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtxcfqde.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cwfdxvsq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2baoohlsk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wdkokeel.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2imisqoxq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vpawtfpk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fyeckgce.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bacvpyfd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qnildhjq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mooxtkds.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2bahzhfbo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2flsappft.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xmumjbwz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ryabzygw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2nkehkovy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2teydckay.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2noxyaidr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2xfeqcezf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wybhqiib.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ozbnoyjo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2eskvvxpn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xrtowdus.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2amngiyek.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rycnmhtd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vvzgicde.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cxsapwdf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wlnsxnfb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hbpznnpo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hwzrtwlh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2gkybyrfq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fzpdkmki.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wbpnlmrf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jguifvay.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bnhflpib.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sdaaqgfw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sfutzimh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2xcinhlwj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nthgerod.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2xktozvkh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2vjiitfdq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2pmrxuyre.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rwktlhgi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2gcedxjtu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jeonwcvg.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ashrxdga.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2baekdwlz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2sccirchk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mfmunxtb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kqvwufmn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fqyhlrzh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ngfwqxvy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2obaopuet.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2slynszqh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2xvzeewgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hstiqbsw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2wmojgqez.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2hrfzdmgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phgbrtyu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2tdrklhqu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2senhbvsx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2pvbbhqjj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2usgkbkcf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2whfcfgai.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2gggewkpk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2pyeuzsff.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zzlektxz.html


<!-- 参考信息 -->