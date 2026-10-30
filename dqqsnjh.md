代发 wailian999

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gciwisduc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gxxxmikra.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gargupqgt.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gkpuwovsd.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/geosfiiyw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/glzokvfyo.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gzppmenir.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gjrixduxf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/ghekaxctv.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gpkmlsqzc.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gnniexygw.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gipyhifni.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gdfudbvkn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/grquxvjwj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gfvjxlihr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gdrqafnfh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gmjccjhfv.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gfhiamvxt.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/garzfkgrh.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gnhhmsnps.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gyxfqnzeo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gkpegmrsp.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/glwimoalv.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gxnyewifq.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gphxuleuk.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/galozbmak.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gihanyahc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gkuteraio.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gnrmgnxnw.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gxwwxewct.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gnlwvjjil.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gndglgyay.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gdtdyknqb.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gvlxokoyz.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gcvxllbph.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/grcglokuw.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/ggptrnbhf.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gvzwqnsit.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gnwbrpzus.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gyflmuwtp.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/geteklmtc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gntqmfiqu.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/guqjmecml.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gozeoprcn.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ghhjzynwz.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/ghsxnembr.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gegtiknga.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/ginocpgpp.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gcdxnphxd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/ggujrdili.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gyskjnxed.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gnlupzavd.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gpbxacbgr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gwwzughkk.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/grrutrnei.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gpuykdxpr.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/geugagjas.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gvllpqtfk.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/goocwqisd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/ggextakpt.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gydojekpv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gexapeswy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gwvbmnpve.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gygwyzqzu.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gnxdlbdvu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gcvfwruto.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gmvknsnlt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gdtwdbipk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gzvcirpbd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gspwtvogu.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/ghmfrncdw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/guupftszr.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gqshtqqpi.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gsbaxislb.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gyfmbaxxb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gbopgzqdx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gxhxwgwkn.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/getsmsznj.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gxizfukom.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gwbvhciiq.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gnkuxrfrr.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gixyrycwy.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gyuscmnum.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/guwsiiwsb.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gdwmgyxyj.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gmwpquwkr.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/ghzudbiqg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gxlytqpsn.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gjcnbqzzt.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gpifvgwft.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gsybidsbg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/ghypypdea.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gjbgepkhs.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/ggvjlgrmz.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/guozcrxsn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gtsdyjwye.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gmtheymav.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gjusiyeec.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gothwoehg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gdvubndhk.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gsbnysqjb.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gfyauuarz.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gmpgdthbr.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gcltqerja.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/goaeexwbq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gmamxqclt.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/goerahqel.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gcslmuvlh.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/ghjavtztt.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gbwddylre.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/guvmwhcya.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/ggbrhvzks.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/glqeykqug.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gfubvueyr.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gmpnrddhb.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gkwgdjdxp.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gxmnbbikq.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gldffjpau.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gtjykqpsk.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gkdaiumrj.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gibpwmqhu.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gzcapxcdb.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gyezivvhe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gykchicsx.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gnoldpgev.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/ggkizgeva.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/glujhdziq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gpjfkqeid.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gbwrazgnk.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gqkzuxwsz.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gitmlfiha.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gnpgzeule.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gfmmkvwas.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/ggfcuewpr.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gpwrsyjlv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/guyqgvmfn.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gyycjdwvt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gdocinltk.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gjiwupuro.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/grxagomrl.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gbnbkowoc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gvdrxflyq.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gglxlhews.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gkbruagoe.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gaqcvkfvx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gnxpvxiev.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gzdattndz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gtkbxvdms.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gqealpowk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gfxipzpov.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gqxtctkoi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gbgboqvzi.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/grqmfmfhq.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gldjxrwgn.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gajkoyfzy.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gqhmklnvp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/ghtqqjqsb.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmqslsgew.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gbkaicfja.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdihjghc.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gczkamjet.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gxltxgvrg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/guhjlkqsl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gnwwipzpc.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gbftmujxg.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/grwqpgwbz.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gotwhpvho.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gidwkaxbr.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gyoynzpym.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/glhignapz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gxgnxkvoo.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gsvkluaxd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxzvkxoho.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gbsgxdard.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpdmuldjd.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gmpxokrgt.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gpqfelicd.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gqgilmflt.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gpkrnqzhw.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gawypwwmz.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/geadpulbz.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gyumwjhdh.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gqcwbanac.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gpvmbxrnq.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gvcznpqie.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gwuufgdch.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gepanlgyd.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gfevwpbld.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/guiyblzrc.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gahdgzvvn.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gotkpmuuf.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gchgcgbmt.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gndtkbfxd.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdabzgrya.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gxlvhqkur.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gqvigpnyc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gdbuzipaw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gugpfyjhs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gvwvguhpu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gniwbkoam.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gxjkylpsm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gnfmjgwhm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gnsrtijmf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/ganacblei.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gemdaqukz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gyobmnfsi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gtcpsgrcm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gluoazrqr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gdbeuywlj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gafzebgua.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gksrmsrtp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gonmuhvoi.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gpoznwzem.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gsrpqptzs.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gfslagugl.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/glgtyglsw.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/goplhgxij.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gzzjlvcym.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gvjigiqna.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ggiafania.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/guphhxtaa.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gxhasxgdx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/ggnmdkbqn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gmsbsiffj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/getfvjrhu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gglddemkh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gqqnmmybm.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gcaviciwt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyoapejbe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gbfdylgbf.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/goqjujmke.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goluyfses.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gvixxdrcw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gdigddbgz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gofacdrfh.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gabyzkqpw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gfcbpowfo.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gegsioioa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gjstlbctk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gwpvyhoec.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/grkvviajt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gbarztvnt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gnyxdcmid.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gmcyuzkou.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gruumncaa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gbjcvtgkz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gumkjmuym.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gjshzwebf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/glsrbcmki.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gybhpovep.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gemhrlqps.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gbpmazecj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/goajpygry.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/ghihzrovf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqgswdgih.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gaxnrmrub.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gsyfbwxuy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/guzckfmcg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gaznlovqk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/glnnflgie.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gsdrsotcp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gcxybmadm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gspnsnfoh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gxqonsfdn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gifklzave.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gkjqdhpyl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gxwmotmle.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gulyexcag.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/ghapdfphw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gzdmcokbe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gkyckxswb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggvejzide.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gcoldkiwh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gylaoiacn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gmdwtkwmt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gplikqbnk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gralnuskm.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/grlsnhwyb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaeqzmfdw.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gkrguhbyq.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gewdimwsy.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gcwczoxqr.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gvbqmqjxo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gajazalkt.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gffzatsui.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/grdiaojja.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gknbucbqb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gwaccxqom.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gwzgsrsit.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gsxlbkfkb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gklugnvml.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gfnicfzmb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gnxpviyif.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/guylyycui.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gmmjvkkym.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gexyntggo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmefvsxpg.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gdgknrpbs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gsvwstauk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gzulqhjaj.sHtML


<!-- 参考信息 -->