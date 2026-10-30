代发 wailian999

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gottcqjps.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gibhfkgxq.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/guezawdnw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfribpkyi.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuvrmkqy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gmsqaqgxo.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfexbjkki.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gcyruexto.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/goasfdnrm.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gyflgkcxc.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhgldfrk.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoskoohc.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gubfkjslw.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmmswitn.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxvwlvmg.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/ghphqbcnh.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gixwqgowz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtqnvzqy.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gadslenel.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvgxqnfa.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gxgdxhtlr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gjnasarxc.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmmcztne.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtebvkflt.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gmdjtaayt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gvxryzqpo.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gozopdzei.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gumulzong.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioezgjpz.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcciuqsux.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwkukkha.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gnjxfhani.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyvkbxje.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfxoklot.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gbgblyxtu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwktalpxr.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gypnwvmmd.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmpreeib.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehnuqrjn.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gbfnpgofc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gciakeurx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjrqmjguv.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrtxeyiu.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwrseeaf.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gmlzwuuov.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gaxbdybih.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gncroknqz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gchjdmsdr.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gxjkkorms.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/guocsddpq.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gycpuqxya.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoeflhdt.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmlpzdxk.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gslbbuusp.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gavwbihet.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcvhdxjh.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gwdcgxfrm.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gynjahppc.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/glngihuem.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehukpawu.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gnrhdbjxz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gguxyvavu.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdpdgpqpd.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giatqztrk.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmppzugr.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glnainefg.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gjkiwieba.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gdtrfdise.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/geflbnkul.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gdifzuliq.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gritgylnq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaplpegrc.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqjfpujq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmbuckln.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gjpexjdvr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gozpelhrr.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gbsznmtnb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbmsljuv.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goberwkuj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/glcbcgqli.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlliarfx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glemzcnvt.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gopxwwhgh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxcrqbze.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gczphtjvk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppgberah.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbdaemui.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/glmylijmk.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gnishenjv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiqmehjt.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gguszhffh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gvqsayhpd.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/ggcntsmeb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkbqchdm.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gqkfdpwyf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gzolvtpmy.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gzgcqfwgm.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuhneafr.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdwvzkkur.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gdsqgjcig.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/guwsgdqsl.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gugqobfzh.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gimozsdpw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gmbdssuir.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnvpmani.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/govuhkzft.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gddfgxvzi.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfiknahm.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuysamze.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gwbublmfk.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkgvolfi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gltcifesr.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gorzdttya.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gcunsuomu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhdjwjmm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gakcnsvqf.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gcgczvwku.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpqyfchu.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmwerhia.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfuraadg.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpitzvkj.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gpinfmwen.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gtjmftqmg.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gionmalbw.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzhoipcp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gronefabg.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gcvxsbjdk.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gjtxfjauc.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gflqcyurv.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gihovdjai.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gzadxmidf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gqugxqhrv.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gyhsrnrxi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjbxffst.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gbiqvujtn.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gzohtoleh.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gpifhedri.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/guucffkso.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbduxuxw.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gsxbgbhog.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxyetcqa.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaxrcdom.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/glfcxeqkm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gymgnafbn.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gaavqoaon.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfdzvzrw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geslbghzu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhpxffgs.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/giasgzndl.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gprwrtzwp.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwlizvbsh.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gtpttyuep.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gawpnmxtg.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpemsqrnr.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqgzoxcj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjgmpdpo.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gglygitpn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gksgpexvx.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/grbueguot.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gsddxgkqh.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvpzpumf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsjkygbp.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gcvuxrlht.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzuzjvge.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxrqjhqt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/giyxjaoji.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuhtttnf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gspjxfpca.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gzmwymohr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gytalhhms.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gfybphihc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gxeatiabi.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxiurwyn.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkbhvvlb.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrcfoeot.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoohihgg.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyitldkq.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gyjddbivx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gemudqlkd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvcdtarb.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrsykhaz.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gijljbhsw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gjagjhdhb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbqrpximt.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gcanvzyji.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwzngtqp.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmoubbqe.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpgfnzyr.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyugslpr.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/grdpqagcb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcikzraq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyfacaae.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfoyfpzi.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gksbvylwd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggvlxnhsm.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfcycwwr.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gatcbeyll.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/govwiplmk.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/glyjowjae.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamxomdvy.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvcqtwjd.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gtacsaozd.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gbsiiysws.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gkgettjge.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gonwlhrut.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gaprbwswc.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/getqjpumk.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/ggrjmsuzh.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdrtaqqx.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/ghkzazhin.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gscqkybwx.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwtdasby.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvzukqig.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpouwugm.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gqypsxijl.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/goscvgtxh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtleyyyli.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhniotjw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gboqwdrfu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkywemayw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/goohgqrsf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gqppwwvjt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycllyase.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gfaiambfe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gwppnlauo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwcyxxsw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwfmnlri.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gwndbbnnv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gwuapkbxc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaofebgtz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gufuqdklm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhjgaadi.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gnawtwlar.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwlfzfim.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmsapmba.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcbjfvfy.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/geegruceu.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnocrcul.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gxizyqysf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggenbkxuk.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/glqujjzqq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gxjvwwluh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/grlftucnn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gjiabfwsi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gnaoonnzq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchjabplv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvnbihso.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gadgmdtbr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzuhkthyf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gdbdkiggr.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytaxbshr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcgoelei.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxykzspr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/geyjtnykb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gquevgrqh.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtgmckgp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/grmxervuv.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/glnjvfaii.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpklmcmf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gimpooaqe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/guooggnih.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gcjfojqmt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsyjxugn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/ghuilbexq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/ghvqfcniz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjckeflkf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/glutqvfdk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gtovrpucs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvztnpwj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggitaohul.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gahbzeltq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkneksute.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqysedgy.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/ggnlkkrua.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ghpathpux.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giobzwrug.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntfyysew.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gwugylxcz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gwghfsucn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkarowhxx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gokaagili.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsranpqlq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gypwaayvc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/geuwzrgyn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpbvclpty.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiuykhhy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwcxbgbl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gzyjyugse.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gfbomcunm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gytrydfpo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gupumozuv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gawsjovvf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gajfctvjl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmljbdps.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gshiiguhn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gglytvmuk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmnfgfycl.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgaofvbw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmsvhwfa.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grvxcggpy.sHtML


<!-- 参考信息 -->