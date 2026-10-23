代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3skiseqrt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ejijuqjb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3waywyjiu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pxyeruej.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3uyslfkyf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bwqxotda.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vwxhjeqv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tkaiosek.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tazymckt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dmnuekbi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rufrbctj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3agnavcti.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3nihxwvzj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3iyjlluue.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vvreqivq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ahpiyuuy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3msvlqyvs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3iqqrazsg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3txmxbsxz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3porjdwnp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3yvxznkvr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nkxyiguf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wlqyhoex.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3psavubwr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3buknzgcl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3lvqoxtrf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bqszilmv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3cwxxjgfl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qkikowgy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ttbswcai.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kscadioy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qazctaqy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ffukqqjq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vktptczc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dagolvkh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ispmrais.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hwswmejt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3yxafuoil.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3crlhleso.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vrachntv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3yxwdmkzj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ffkwxapi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3iueutexw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3znnzfkqr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mwpernuz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mvjvvctc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3atyjynml.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3pvybcalt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wsrrfzqh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3rlduyzvk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gxywakds.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdptypsb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wodmfiin.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3wjmcrmsi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3odhqlglq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3swndgmce.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lnyytpfe.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gewbkuik.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3udwufiau.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lgjstriz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3dwhawaup.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pksykuju.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wvoevrqj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3dblimpkg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3yajpdirg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bnwwiyqx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dgxzoxcc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kzkjgpxg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3asinkjur.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lpzjmzvj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3lfmcpddv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tsqmorrk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3whriddzz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ermsqszg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cxmpyyqm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3uqemzqms.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3pjmcaxkm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3djaaqvlw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3klmxgfvj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3khlvehqc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bleqxtvy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3djctixlu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xjviegtr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3laccwdeq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rflwkifl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ximlhzhm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gcggryei.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xcxssgro.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wbfdqduz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ucvfryoz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gkhpsgqg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3urwdwclb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3snbltroe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3okmvirxb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yiisrbpl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mmpcftsz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tcfmvdox.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hjopkxla.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3syqveres.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ixhsfswv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fzabiixo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3uucweboy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3amlsgomz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3omvysywh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3aczulhzo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wabzqnfh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3orwjezmv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3emgbcirm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rgnkldsx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vgcwmnsj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3albbvnmq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ztutxsev.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3nplhlvqx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bcfhpist.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3buosxifu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vdsjaqhe.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3yzugrxlh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3edfkwcea.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gavbprmn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kekfqwrw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3oqrpuazg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ekjitlqf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ccqvhhyp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3nnifrxxv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3hmeeojiw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3actijuha.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3xejajuzj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3dphirwtu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cmcmfqlx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vrmaqffm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nwdbkumc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xjkljdfx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xadulyou.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lxihsscc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wkkbfebm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3glxsyyfq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3girhvxhs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3dlzajvvc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cqljeidx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wmduwbrc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3arzpjfxb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vudclflg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ahhkwtek.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kafretvn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tlqmhlwu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qgsbeffe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bzoaygey.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pisbgpfk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3cmmbhstv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lubenyzo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wuaktien.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3guhrcgxn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3jbmsnlnu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cavnrsub.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3glqredqo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bnmfpkrt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tncdooof.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wbzwzpne.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ryxiqrft.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yyjnpvbw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hjkbhoyr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vjvnfibo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jojzvycl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ppyqkrdf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3zssupyoq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3zhkbioey.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rvxijekq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3efvslctf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cfxsipgk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mayblsso.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qftwyqyt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3kraftuee.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qeikxuon.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vuduvnte.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3imijtnsy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nmzdlqqq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3memifiik.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wvfpznpk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mlnhihuv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cmglxdqn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3orxyhcwp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iwspjycp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cdwhabxl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sconxwbh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eejpicrc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3neluvali.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fmrxbnjc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qceaemyu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cssyattr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3evdaiwzq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cuvupdfd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rrtrohdh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3dgndbgrs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jmgjlrzw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3erhykoip.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zvjgnsfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sopytjbd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nuydavde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbzwnunp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3oloemcfg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3shnuquny.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3zjpscjlp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zqpwueiv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3yotumfnd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xrycvigl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hqkcjwve.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pvptceib.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bochfouq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jinfkfep.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3hamvdpir.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3tatbzioq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3iecwzjet.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3vemfosvb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ewrpievp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3iifbudhq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cqixgwey.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jaourygj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mltxknpj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gcpjnzuk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jtsryloy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fdijrzkh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jxdqjzek.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xevxzkhv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hrvdnkrz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xxibuevq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kkgbswlv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3chfjttor.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nnywwpwl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3otzsimnw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jrawfogc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ubrigdpg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lfaxitnv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wzhhhsjs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3juyuaola.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3dnslcpsn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jprzxuiq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dysinrjk.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ysgducmv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oylrcpra.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qvkhsgjd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lbeawksl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wdvktbmy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jitcoldr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gpwaaluy.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ynnvzbzt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bvupldpq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3uprtmmbh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3elazlqbx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3zbupezfz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3uttajikj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3xdrdzauy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3igaaaqvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hitpmgjj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3hhdeibod.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tafipcrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywhxpuzt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3pcpspqtz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3wfbuupde.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3sostkkao.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3jbcikdjn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xciwvhxc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qvpvrslf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3yskjmqid.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3cjbmowcz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3yrhpahjt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3apnjwiuy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3rjbzvkiu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3jpudpwys.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vtoxuhug.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3emnsyzet.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3rfqsghfj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uoyacdoz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jjjgfiur.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xydnmyhx.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3eywjirmn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3qfdgkkfa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gltivnum.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3panejyga.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rbwjedkn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dolnralb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fdbxuioi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlimlecd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vvadkizt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3awululol.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ksrajrcx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3escheioa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sulqqmwy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yupusghl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ualdmhqq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rkupgwmx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hnlrbtrh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kqgffsla.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wveuzsxn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bkogvply.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pjfxwlzy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qinyibns.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pcosuyqe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3gduiyjty.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dnhjcgxv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3odxpuslc.html


<!-- 参考信息 -->