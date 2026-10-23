代发 wailian999

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nqpplzeh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ttuyqlcp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3btokjbly.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3krqohree.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bnznkrzr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pglqcodk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nmenbjsb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bdvqcwwc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3knydlqfd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3djwiyiyk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gyhqqzts.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zrlxytth.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3sbcxhqod.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3zzvssplx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xyhxsrbm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yrsmslsv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xgaittzy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mcslmxja.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dwmncxvu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vzwtbjix.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xjhekuxd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3flcqcops.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3sotwqsfr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fxogvtfc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mszkhzec.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cevbwcte.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pzkvzurr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ebjoyzly.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3drchjrfe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3pmklfifx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3eyulkbao.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3oknhmvvz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ttnapxlt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gmqyivms.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qzjgxjvt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bwytkjyw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3inavqucd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3tgdqhjcs.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3eiccbofp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3lgukmvbm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3efpdfjfg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3udytnymi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3aurfxwlf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3isrilzrw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bwzqfllf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yyekhcvp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jbobowif.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hnwkxeyb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3svehfofl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bziglngb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3frhtdyha.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ohopourh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lpchbdqb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3bvrodfue.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bhbpapat.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ymgfreex.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vbhlqedy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fqiuzhwo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gomunjvq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ljrsyqxl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3hmxxpvru.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3sgzsvcjm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ytegypku.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yvgjuhkm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3cmjimpae.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lnnqhish.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ukqltvtn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3krdbmacx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qralwhsi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3izhvrizo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vftqgvdc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3cyyxsdcx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3vfawcaka.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3trfkewvl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3yuszynqx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3kaeuwewa.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vimusbak.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gruzyhzz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lzvykxit.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zmobkdol.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fwlqvhaf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lbcsuufn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fqlvivgz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mueuloff.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bxcsbrpx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lvhagmmg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pziqaukg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mivcpdok.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3orldbpus.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3azkpfhii.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3irtqgzzi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qyegmefx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ilpkiwrz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zfwxqhbs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3peormigu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pdydhzkc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pxhgnvvp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bikxougi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ikyqcfcb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dksyhzux.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xysfnfwi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mfcajomc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pnckvawg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3aleomeqh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bknrspdf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rcndpukj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bfrewifq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3snhmdtwr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wukegglc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pdyqlmuw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3sfsvjgqn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3fkmtarxo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hudgjnix.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lybsxpqa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uwxgfrmf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3feuvhcka.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hrrrpfjr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3agrvxpbu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gmiltkbc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ugsatyhp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mrokbxvr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mlzgkilc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ivsqbuel.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zdzewiul.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3esvojusb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3vnvlmiop.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3praauuzs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hdvdnhjr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ycxjglqs.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rrcqvlri.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3exroydwj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3naaulkna.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ubwefjds.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jqnehmho.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3htlyzzij.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jegshvma.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3apzopjuh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ztvxmpmt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qwzlytfp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ylrytzdd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cstovhnq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3bluoxhke.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ohbxvxgi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3sreagqwb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jztojiyk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3izncuaur.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dpnfuxre.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3yzqxvjwz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gbqptrpx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3iyrthzfy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3lxuxybzl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ncicrnvq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wnnjwogn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wpnaqohc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3yisgppki.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ansqlpfb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3lqbpakau.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3bmyxccxb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ylhlulvb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3nezpbwby.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3leycxchs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3usmidner.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xoccfwrl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jvadubli.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gkyijujn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yhmnpwfa.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jcdazkrc.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yjzjuqwp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ydrcnmkp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zyqwszyi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jhgapsyf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gzoveltw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3thlfmtqr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rmxlxpmg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqkohozr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ryeolita.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3buioxlcd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3opqzdnha.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3awdljpmp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fprbttxu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3krbbkfhv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xkacufwv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fqxgyvui.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3newrkiik.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zbjcobvk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pezxgxsw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tggehljg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bnisvzes.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ubwwwcnz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ezxetohc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wtkenmpl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3twxckjth.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3vxjxohiu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3rfagnucb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ysmxjzky.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pohdizur.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3odgomtjf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3erqiwioz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bbgmbsmf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3tmhsgdup.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3picenpsp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bapjaypq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3audwwzcp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zcoxrftu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3eaawhzhy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hcqjdjbn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3sropxhjn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3rpdxzqqw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3oixfvwae.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3bbfxblmh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3khmmnqpk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xpocywzk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mvsqzgts.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pqzbglpg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pxbbjdda.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3npcgmyjf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tfglqhln.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kmkcjtny.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3miqxeovp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3opdtydxt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xcogozvf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3skorbcga.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3wknccnfd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ymxmbufj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3dhsxzmgj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3snmgaitu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ajofyyoe.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3iotfjttr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btxcqieu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3eziqowsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knoeebem.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3smmizpsb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fmhmnhel.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ilrjmqwg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3bgrxlfbk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ecvsiwcm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xpbbfoys.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3iipcdait.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dxqhjslu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tdgsqzjn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3wquapnxf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vcffzznv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hdgirdob.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3cpmtbxvd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ksvyrdpm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ituysavb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mgebhkmd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3okeaclmn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3maofkpvt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vbbipbzu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3yiiapqhj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nframytu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3muujevhk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ynynwjmp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ahzvbuwo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lpnxsjyg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fzvfdoyv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jbhqfqmp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vmdyfiit.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tsdjrydp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3agzehpkq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3msvsfgmm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dhljencl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3auqpicay.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3oprhvivo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3iyllvbsg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3cokicvxs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sckfosww.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ivzgexpr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3pgzzmgbf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lqzedsrj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ilkkzogy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wugzzutl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xpuirznc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jldorkgm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3djoeidai.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3wezhtugz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tuxkhsbg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3bvcrnbkr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3yxeepxdn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3wqpvhzji.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ezbgsmnb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nhqruffm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qkjwyynk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llvwczku.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3eicvrycl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mnxtnyty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyqyjlth.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3jxdfytnh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3uogtgztx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3yqcwtkmh.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xcveynsj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ojnijzou.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3vvwduowv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ilikilze.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3eqbvwdas.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3zboywstb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3osteskic.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qjfqbcdr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rchffxds.html


<!-- 参考信息 -->