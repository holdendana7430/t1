代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gujtnavim.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gybpwuskl.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/ggmqqquod.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbsmghl.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gtykqodsf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gzlkpskvf.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gswejbssx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gammnkwrd.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gwostzqlf.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpjctmhq.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gefcwsfhu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gwdisjrqi.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gdmhdemuo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gwzygqpkb.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gagkyoifo.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gfeolvkuk.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gmjxauuqr.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/ggcfmodox.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gphdrgcdu.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwwdanbz.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/ghulnrscg.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gejukgwmg.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gdbxjapqg.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gsbahshwi.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gkecwnmke.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/glmfigogh.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/ggfhoaudh.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gyvtecieq.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/galhqzbgu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gjunvolzw.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gashsvvsa.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gpbxqrjhd.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gzuingche.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gyihsdegh.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gxtysjjpy.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gmmmwhcyq.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gyyjveyni.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gvisvqffl.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gbxhgcetr.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gibrwupqu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gnsvaexhg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gcijeznaw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/grxztstcz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gnanzpoyg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gfrirdnrx.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gsoporghj.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gguinazue.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/govdqipll.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gvmvoiiil.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gagisoxsg.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/grcpoowuz.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gprdyqkzr.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gqgsvbsib.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gxnmyulbp.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gxwmduypc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gvnejiuwi.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/ggbfypsqs.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gmzpapfiz.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/grlhqattu.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gbgtxmqam.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gwiybjxlz.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gweezotcd.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gguxkiexg.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gknoprrpp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/ghgwpesoc.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gnjxvpbww.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gcrizmopd.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gqgnnhklw.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gcsmheytl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gxpjxsekw.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gifmzqgbu.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/getiklmyn.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gftpbicow.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gqvpjrtvk.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gidfhnmmu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdgrjnonv.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/giwbzpvno.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gplehgkcm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gnymajvmw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gzaoxujlg.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gsiaxmhjm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gncwcamww.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gpvlruogx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gxnmufjtk.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gpfhavour.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gyvhtbvvw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gbejjswyi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gozmpuzhf.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/ghuuacpts.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/guweqyxll.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gmcyyrnvw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/grczmzdba.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/ggzopzinz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gpfspdugs.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/ghredbcgy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gtwmiofed.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gjxpqernk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/ganvevzcg.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gvdnzsmxa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gtndftxss.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gqkobjidc.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gjmttcpud.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gaytohiqm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gngexvell.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gmopqfehg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gekieefzk.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gkoyyixfi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gdyeiqsxv.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gpborjdyz.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gvsbxdbcx.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gnciwbdek.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gtieqeeto.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gwcfmncaq.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gwyllkgul.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gsdbafonc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gjzknpxce.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gwktpmryu.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gujmfugrc.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gfavqxdrg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gldhhzpjq.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/ggnywbehc.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gsoeksqup.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gczehiozt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gpuzzzgbj.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gnusarare.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ggeuvdckq.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gjvikgopn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gafulmjxa.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gqxyzqteb.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/guwqgwzyz.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gasmzrfmv.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/glyqdcrga.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gkjtjdusl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gsfpyjsrb.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gdeutayba.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/grcirolnh.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/ghswqxmfj.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gvrfcqocu.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gwzvcabcw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gjvytvlzd.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gctxithjz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/geiuwqcqg.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gsfqyorun.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gfkwocfns.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gygcgfpxh.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gohbmmhxj.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gubdsoudr.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gcbecrdgc.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gycokjhfz.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gxgncmsbe.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gkwlimbog.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gvucatxpn.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gxirhlspz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gugawwvmh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gdujvtvmg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gyotkxksl.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gohvavpcb.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gtkzkheco.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gtjhgkzyq.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gwkqzbgcy.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/grwckqvtl.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gyiqdyjmv.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gclajdnhw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gbdmpzyqi.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gyxfciruv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gthkmvbug.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gezqtomhy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gjfuakexl.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gsyxuofbt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/ggoejyyxd.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/glyorqyfb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gpmuvjywt.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gfyygjyea.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gvcmfpkgo.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gunvqvvbh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/ghcppplsa.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gyutkckvz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gugqmmzxd.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/guocrfzff.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gzhdukacc.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gwotuzvuq.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/ggjvocrdc.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/goquckwws.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gkoxefymr.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gvgibokok.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcrvesiwm.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/galufubrp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gadhnprdd.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/ghsezqnyl.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gbznhopwm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gxmdsgrfb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gbccowjyy.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/grywjltxj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gfaagqbrf.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gsvpurnss.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gpsndxhgk.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gjtdfojlp.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gwekzjdir.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/grjusnfpj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gobcbsxoo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwiwyvoqg.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gbcwchyrj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyrxtdask.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gknkybwkg.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gxjhyjzyt.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gykrihuwi.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gvgsocygf.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gqrqtdkbz.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gythcnify.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gbytioeqq.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gqtnjuedt.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gacrxulme.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/ghecbdfkk.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gmklxttjb.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gxsczxudi.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gowkfhmoz.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gubigpzdq.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gijhgrzlu.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gmexnlbfv.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/giqjfsjfy.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gzpvfrtrq.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gjayellmo.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gvljwwccq.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gusbpufpg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gcotndngi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gzbzwqrgr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gxpojjnxk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gsbjrnsxu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gbhecpiys.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gykbwwwjg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gpoeeecnd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gnaencgmc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gjssygiqq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/ghrjfqpja.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxiqzeree.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/guombqggt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gdfzmpkwo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gbgabkytb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gcjuoowxn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gohjakbgv.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gcowulgge.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gjqnlepdr.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gitgjlhab.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/guyipubxk.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gecblikiq.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gdcmkpdny.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gkvjeumii.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gjkhwtajd.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gsglertsi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gfbjthsyd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/glkjymquw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gkuywdkob.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gqqklgsjz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gzvviykjq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/ghdndygdz.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gubsjbxeh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdaxskveg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gdisvydvx.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gwxwiwfvi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtujotily.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gefasxyqq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gkacssgfn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/goadhxefd.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gyrdmjlim.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gtzvsuqct.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gracfplut.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gqlzciclj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gbqfajuyk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/ghfkijcuf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gbxmgpyds.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/glevqqqef.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/ggtwiazkw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gaunpvaun.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gxnwrsfga.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gdyjnjmjj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gdgsiwhvg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gyjdsxdmg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gvxecvuhx.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/grpbhmntv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gwwrzswdq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gcesmqitn.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gbeuoucka.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gkrjaxjpl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/giljhjlup.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gbnmijxnw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/ggqswywmx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gpjijljhf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gzvjitszx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggoqikndj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gkqcpehqr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gikmaakim.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gdwaqdsmf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gbzgghovh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gmepyvova.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcsfgzmhy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gkzcgoyns.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdxfpqe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gsbkwlfjl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gauycajiw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/grrfuaasu.sHtML


<!-- 参考信息 -->