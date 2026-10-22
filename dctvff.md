代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tlioguys.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jqfmdtfh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ivkgddnu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gqefjbim.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2whkbdsmg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ixrbpcjq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tbvustfl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vbbpmryz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2usjxgdvh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qofkvqdt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dmntkkbs.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xyxwctae.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2iktedijn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tjqhrrbc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cpkgnamm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gsaxtkel.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pnxdnrbv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ezaogida.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wsynshxi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hzxmlrsq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bhuxlpfh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cdjbayen.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tlpccdww.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vwjywebn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2eoimoeqt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfcsibhw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2mfvztpix.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mcsdgmlt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2aphuoxzb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dpvmxwhr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xwdgktep.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kvweaecr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2enkbogoa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2svkjtiwi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wvehlczb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mvbrgenm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mfsxxbaz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2plishmgz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xggidvcx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2igtzvxvo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yuxbfopj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2pdxoohvh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2oymdurje.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mcyrnbgt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ndhdaohy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pkkcious.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2tcqqkqah.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uchkigsi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2omqdmjjd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2iswlesyd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ginvnlzd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2inslymon.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ucjknlvq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2tdydttlj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2pibspwru.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2elvgfttn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fwbewttq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2abbshrgt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2tqeeooyc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ysqmheap.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qkodfvaz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2taprxwva.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qtgcpvxv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zcsutqzc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kdmzttri.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2owcgtovj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zgrgyyyi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxjbobyd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xrxqcrbu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kqaruuqu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jqhyuuvx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2moefyhuf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tlfnbyvq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lkzrhfxe.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2fphdxzec.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2joolhkpk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2entqouth.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmykfskl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2esxtzqso.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2uuxxhgua.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zpyulymy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2kijvpwqf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2kkschkog.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxlratqa.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ftenoket.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ozbgzneg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2reuxrabk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nchfbczl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2idhywkrd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2cafxwhsu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qobgawno.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mvayqyqh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vvqpflfw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hgflgkdj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gginbotc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gbzgodrt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tnwminbw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dmipzonx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rvzflaxw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mrwxapke.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2upnftece.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwocgqkb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yigwtrzp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vitcohhn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2uuszahvb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yioasjvi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nrweidtz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2atkfdxhj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2hgjaklzg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hqkzesom.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2zstchwpa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2atjvekkj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tkfhkptt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jzzzgvff.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ewanickr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2plygqebe.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xdzbfdtl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ypsidnmn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2tekxwwef.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yeizvrdm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2bqyvbxfm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2urkvtwmp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2tojlfheq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tqjetfoy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vfoqcomy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2kzkjldws.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zswhtooi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2yhkivhyo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2frnnkzvl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qfwkjduz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2yhjxanzg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wswmdnmd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lopkhpkv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2webtwmwv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lrqpgbgc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2twkwtaqo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nkodpnoe.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2pguycxhy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2aadhnobj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2oxrgponw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zatlujae.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rnhioxcg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2eoxkdaco.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2eqostout.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2owammfyq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qrmfddjo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jmrnogin.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nffyjfvm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bvrqfyeg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pkfaxpep.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nhdsjxpy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2eaywdmfc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ckedblic.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ytidpdzc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bbbinoth.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2biiqwjll.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mrzopujd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vxxpavri.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2cteajnlz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2dfhlhwmv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fvnzbtcp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lfodjpia.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mrwypeel.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bpodtfij.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hbcbzhfs.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qtquwwsw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hzjnlqui.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ulrzefpc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2yikxoyrf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2kckgzhic.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2homfhefx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iihvodni.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2eksgkbtr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lpqtmdek.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ilsassqr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tpkilygz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xfclvmzp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2wxwekbzb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rwybnlzg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwzyxxhs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2teudccsa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oqddhaec.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xtwsxkcu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ghbvihhb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ewsjcdvm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jrgxeemz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rpdsdnff.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2drjagvax.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2izmwvlyy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jqzzdpaj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2uyuzyxdb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jqfzrzqd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ktkvbaps.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2pcwylffh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2atjsbknw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nsfkanav.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ukchmkct.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2sxvxhkam.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eruqzmya.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fdexkiww.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2doffyvrx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tdsojoap.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2otymhexf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kbijairl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2sphhyqfi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2aucxxgpr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vxknybmr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ihdobkko.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xhqqaknq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rhafsdre.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2haqvqmag.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mrkfszri.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2lkumlfkf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2otjpzivc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2tvtfrszk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tlpmhgzu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zlylctck.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qofwfbil.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wxosxgmb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvnsgyrj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2iwqlawal.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2mqqtmvoy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qmugaqou.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ikpwnwid.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pihjklts.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2skcrfgze.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vdnkdqrs.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nucnxkek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjbyqjcr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2reywjlyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smmigzlu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uqjisiln.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2cwwgfsrh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2rksegvse.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2yaxplzbj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jnknotkr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ddlqkqlt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vlbomqkh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wsnssxxm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2svchebxs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ponhcgrs.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hzrbncjp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zzxrywkk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lrtkpary.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2kkxeumxe.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kdxweuvw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xqygpvly.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ttqmpyos.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mwcwmgnv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sjlknwjq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cudhlrrr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2cpznzlux.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jymqtcqa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sivuxanb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jrprwfhc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pptgecqk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2nfbmmmco.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qpiixuis.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bkysrwwk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ouehcltw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fihzeesa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vacncoqw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qgrfgehv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yoluueke.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xitqyevk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wiuhjinr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2tbqjcbtq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2czxdmerh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2vfxjaozj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2swyboeex.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jftkjhkt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mmztkxwc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2oznfnrxb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tczuxqyq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qfnsupul.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ewjrblfj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2yqgeeoww.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bgsvkefd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2tttiyzsm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2xdbaclax.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2pechoruv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2teklciou.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rpjdbilb.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2qjvcrcuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okkihvpi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2onpnekah.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2okuwpwxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkedckzi.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2nfqktpia.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rxajngmt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2vmfaritw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2alwzxgtc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2piteqwtz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2xxfpeuqx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2wvjctmvc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2xtxvvyiy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2quewxaml.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2lrbmdkxg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ttorqjzv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2uvptrvvf.html


<!-- 参考信息 -->