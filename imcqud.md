代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fetghjik.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tyisbruf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3njkbhwgr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3menlpnsx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xyqkxsvn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rexfnlcv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3iqhgfwdw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zagzakqk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ldbkkkym.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bovjbtxw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3kunusvob.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vilscbax.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3sujpunec.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wcygfuep.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hxtgwawe.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wkaelbly.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3eyrdigkb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gnfycxhg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iwetwqsq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rfpiyapb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3snjdyfye.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ptbzbija.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qxzieplu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jtmoaqof.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3iuzuwibp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rcusnohk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3didquhee.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3yjyptbbh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3kzewzwmh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ecxkplkj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hotjhroi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3cvjqxcag.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3hjermarq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3srnwjlyo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vpkkegae.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zlmsmbat.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ptsfwmjs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wdwtpppg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3whhgnznk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dfifszds.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gvxyjkrl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vugkevbg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3htgwmvwi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xxwlvksw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ybbxrvof.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3riuoatjm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xuzhqmeu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3iddeunsn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wjwaujhb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wedcdmsa.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3gqxsrxdn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cjpzdhqt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zgjqdbuj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3crbihtlf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zflwxmat.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfbdsgjd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qttxpsus.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mutlpdix.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ggsfjcug.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zvkzufad.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3gcqxutin.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uyodmiuw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wnqtyyrh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wuvxmibn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3scxtmuoj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wnbtuzpm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ekvwrlcg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vlbaeofl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kotlvpwz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tvorkkkm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3aomznxai.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uotiklcf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eyqmvzao.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3twblfmgh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nxocrcto.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gyiucxye.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3suebcqmk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cotijbkg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hzrwvmjm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3uboamrho.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xkqlkhwu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vdxyyifa.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ymzkfqgk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mlzglqxv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gyeaajmr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ckyfoiet.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mxcqbxqm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3uvfpucmu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3myxohhws.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vfrhxjee.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ikyhrxcy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dkkstqiw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3volzhjtt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mjfhzufk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zsfykxgx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3eimmuwpy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3vybcwjlo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kmnlzriq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ubcuyjrh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kdxxrlxi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hqaxdyxg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ptfqzqqw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3tphyrbtf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mhoonaga.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bwucqgdi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xnwhmieo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uflxrcnv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rcvhykoh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3eilrogcb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bylabjhr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ddarulcs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3rsigzzmd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3nhdioobp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3kklferto.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sgvxrqym.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3uljnnhmm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3viqfleac.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bxrqrdbm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3swrzqzdx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ghtdfnqh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3lyoqfdnv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bclzhiic.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xrzlinhx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3eqndblmb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bhamceay.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bihojuzb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3lhlizvdx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zibeunmn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vknoxsit.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mleajqls.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ewselsjf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vqbsjmca.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3sijeycqe.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xeyngqza.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wxviflyn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xmvppnaf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sptjgczw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kbghdaiv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3efbtdcjx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fmiffipl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3euhvmcad.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3doahocnc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tstkysco.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yvvecjrk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vymdbkvw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vmltnswc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xzmvcbhl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wediigjs.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mgtpsezo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hhyglggy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3mtkpinva.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ictobzgj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3twuqscxk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3shocngdm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cgdndgjz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rxfpkdmh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3lndmpqaj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jguuacmt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3giqlfhkf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3pflvzqup.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3agzycfys.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ioahtilj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3nnomelce.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kvqxwfyf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fsgebflh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3brjtidlv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fshjjdta.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cdmbaavz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3clepetpr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3lxuehqbn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mvosmgvl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3sgjjskfs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3awtgttal.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ajqlpbvz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pdwfuwnq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mmvczput.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rctgklij.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kyeooqiu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3odfkhfpm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3togdtfve.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uyviutuy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jjfyonsu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kgeiqjjx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fglqypul.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3sxpslehb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mclxpvnx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qynnvwnu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nslvktnk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fihujfgm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3apyztorf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xtpmnflt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugqigshh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vzcouqqc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3nlfyltar.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vpddkrlt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3cjghlrdm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jvyijytp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ogkifyng.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jafztqdo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3igvptxmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dutcvhpu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3cbjmkcjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrulhudp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rzapwzop.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jmsvmoaz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mqcflfwj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3bmunqayx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ofpdyidx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lnxnaore.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3icvwdhdm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pckycqyz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pasqdfgk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3frwmyyui.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3phtybaiz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3jiqokzqt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kwfrhgrr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3gneqcgra.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zqwppfmj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ztrgyeir.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3nrvvilbd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jgenwdth.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fqjkflzz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fetyfose.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3amrruwfk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vynbzjpk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tblkdkzx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xzoetvjm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ffeiiflu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3undwogvr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3aaiudvho.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sgygpsrk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3lnglptwf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qyftvyna.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3oddbejus.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3buvugcoo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qnkuqyeq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tetarvoy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pflmcmmx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gtpffzcm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oxvssjfx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bsokyczr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3tiuezjgr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rdkqtjip.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3bckoccfp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3vthmtina.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ncgfoolh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3glmrmrpy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zclkmlxv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3zzhzhmia.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dzfhpayh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qhvvgigt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3rodzzmyy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3obrtgdmi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3stelgath.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3zuobuppg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3plbispzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pegdqlri.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3edagyrql.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3nrkeatet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baqaaqxr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3knthjoyc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3nyrrzsel.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lljghmbs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lyzdfvgd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3mvqnadcp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bwhmzrks.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3npoznvoo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3pqrmgmvu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3aitkstqi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3fvskepkl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vojqenjg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3zbcuxwcs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3fsrjupoa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3eodprhwm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xrwtqwvu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3lqibddco.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jhkytpyq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hyyurdjj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xcaqeuut.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3lrttqqhd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vqpilxlx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jedzbggg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cmvhveah.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iksyzsao.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxpmwznb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3btrwvfqm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ocsrelcm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3myrfhzvh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cflqupos.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3itvcfrxp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3agnypceu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmzvnpis.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cnxahhji.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hoeyvlxw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uekqqtty.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jhgwvnph.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jqqgffyp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dmdymtmu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3knhwtugg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3botlgijr.html


<!-- 参考信息 -->