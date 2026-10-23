代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sqwgntpx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xmgfbpca.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nllmdvwn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3oqbhiuxz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hqvdqnev.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jalvwret.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tfjphcpx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3xsbpatzq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xemtoiqk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3tmnvkxwo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3iupfulmf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nwbizbsz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qocmsvbc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tculhitu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qivhxelt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jzqhdfch.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tmffeznw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3eclruztx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3lglaacsx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kcorsmuu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vuemfhip.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3glsmebie.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3trehjqqy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3tytbviyv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3clrhavcg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3obfjfnti.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fhvaqzwj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tlwnkzty.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jklooxpi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ttnphhqe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bcmhmxif.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ydghyibb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kjigtemz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ofxwbsxx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qhxfaedx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fvayqvnc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gdmznwfy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3uaxrhiaz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wpzpwpjw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zncuwvwi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3etssenhi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nlwxotzt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gnkcjuik.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vdofqpai.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3sttkmvam.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mmvondzp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3yyjukakn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vgsvoleg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3serxlyhh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rsnipymi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dpdacxso.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vcpxqulb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jmmxizqv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bcrnjlzf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3uglpzezy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vmaffhxh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3kinvxbap.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3xiwvnoyb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rjuhxkow.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mhphmngk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3oggxbmqw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3chbmtuhn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ptwylosb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nfenekzz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3epawedbs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qpignejw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qcrvcqmo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gepqfspp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3kxkdczwr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lqcxqisp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mgdrfsuv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bpcdcjrb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3svxtough.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ckwtxerd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fpuxntqv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3aegyzbti.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zefzxpmv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xwxjwwuj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3spszoxgw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ukazedhw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3jblybbyt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fbfzhqtp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpimugva.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3abcooctk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xrelshoe.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3avvikyed.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3akakwuoy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3yarqvtoh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3pdqfnyvh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vghntycu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tpsgsrua.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxuzlltl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vetfvyvu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hcsmhmfs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbvizquk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lcktogfl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rhmgvkyo.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jyhlrteo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wqgwamte.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3myfguacn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pmeohpye.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hkgfyiyh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3dxdecbkd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tevnjrbf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dgnpqhal.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3uudbajgb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hdvfqymu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kfixkobk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wuzxgqjf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ohywkbic.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3boiaulhk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3xsbwyqix.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vxbxigvf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ckzqdjks.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3mbahumcr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vagnxbhy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3cdsmcohf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hphbojch.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ywwfmkbk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3rgqguhtd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zoqstbrk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3blkmtsuh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ffciecjr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3djxmhicq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zbqrximw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zxscatlr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hmifpwgz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3favxnhzv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3onejriqt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rzerubis.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3kopjzeld.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mogdxgmh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lnvgatqq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dysocvkx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3sezgxdjt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3srhcqdhk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3szbhmwir.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3chnupqvk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oyjtjtsj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3loxmrvta.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3icgzglfx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ntnfzxze.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gclcxbpc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3vajuvaza.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mhacnizz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3rgtoftht.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vqtctrjf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3brmlrhyl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ycmwbnjn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tkxdjagy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mthuctct.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3eopemawc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3kqwoemgn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3idtbknau.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gvsxhmzg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tpmummxl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3igxwhsgi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rhhrkgdv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ilqtpjpl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3atjffyxv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3mzegmtnw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vewdhcpl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3dmolalvy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cnazqiqj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3plljpfnz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gjxtkatx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zkrmnvsu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qgromfzl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ctbniefm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zbsbgdpk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3crrxvgio.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gmuzflqv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3yhlvdjrl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3sysowhis.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gizxuvjj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ymhghcoy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tdwwdsow.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3cpicyfwy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbcluqyv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wukgjeou.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3twarctxk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qcovonql.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wxuvfbyi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjywoecf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3babhqvil.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gmpsjoxo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3nndjpsdr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bbbtofvl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jabnixwe.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qckuvkcz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ngtxdemd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3acgmhluj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3sqvcbvjo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cpepjnqo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3acvdniiv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yghrvltg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3twveyezu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3fmcqajzq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xjgmrvdy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nujgonnu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lnxpblzu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tjfkewpi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xcerawzt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ckonwvrh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jscxruif.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fdrbymzn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3vhkszcgq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3hctuatmr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3oiuxswvc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vxyfpahp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lronsfap.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3tymiivjz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3npejawvd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pabxinqg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3clwtnjmc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uawsykkl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3jskhfhgx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mcqdvgbz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bbguqmot.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3okkppudv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3drdvyboc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3deltbrlp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xowmapps.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3coykgpvm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bzmesefn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3tmzsaloe.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pfbfeywx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jwxlpvxq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3urnrhznk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3yepaqihu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rhzewkjj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jcvcwmel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncxxkzny.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3kbmnrmlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxvjygza.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wpzvweud.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nndfcuhu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ttljlvwl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3evynsgbk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pxpnlogb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zgvskgpn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gacdcvtm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fkyppdup.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3frjzfwip.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ksymndwe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3meoziows.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3enugsurg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qkkiujjm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jrimpqmh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3glnvshej.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3kuaqbcvv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3iuxjlcxz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hifwfumw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zupndjoh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ypyflgkl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wajdagde.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ywwbjmlf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zuespmoo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pdrhujhu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rzkdgbdr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3brciznmm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qkiqhupf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mzoffwim.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3epvijxkk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pxskygzl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3boneclxc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3owfrcftr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jxnynzto.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wuxppzlu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3shactpoq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ivdubktn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rtabgoum.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3arzwdxpq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ajtauxse.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3cvrlpqjh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3wsdwdmfn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xqxodhij.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ynnifnfy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3exrrnioh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lzpllkvm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3thgptfrz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zoqfwdcj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3pjkhrvgw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3dryckmkc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3raxptjsk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ujllnliq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3bhfjfuak.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3tpbkiihj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrsdqgdt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nehkcweh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3gmzxzjju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmcvgdgp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3erpjulit.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3flhslkdf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3fokzmofv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3eaaozepv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3pbiuvcam.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3tdttxgpa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3lpwvzabp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3yxiitqld.html


<!-- 参考信息 -->