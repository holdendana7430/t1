代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qeeszkrs.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3snnoqlgi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kndhrsbs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bxcoufql.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yvlvnbpq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hjwwtrlc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rnnrkpgn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ivtkncbq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dqfblpaj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vkvqinjp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dhjmpklr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ivgywrvv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3rwiwxidp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hgxnwiig.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3revwdkbn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3msbwllba.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wlhceapz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tbfijido.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3awmurfmq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nbfyfcjp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3puleahev.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bvwwebwe.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vkenyfpg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3dlgsewmx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vsjsgpmp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3uinxpkhs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3frwdqcgm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3qcsoiyxq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bwmlrjjs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qgkkkknv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rrzgxihk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3volzvqmv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nilxjbof.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nqgegbvy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ptzvptbj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jsxvswjs.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3atryfwzl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hbrnieyy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3pipajnpi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wupqpotl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qvqfsolv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3drhyhmcz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3azpkrhsb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cttfdmir.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gdyhuqrx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3orwtsrke.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bycvaztx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dprvguvr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3yeodpwrc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fwqdrjmb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3hvoeoaoo.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ygfsdtvf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3mgfvqwzg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3jsbpihhe.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3etawdsgr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wiflexty.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3flvnjwpi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gisysajc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3cqhmtkql.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pmnqidcm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eoskytfj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yltukedq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgsvfutx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xptrhybc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lsibwsap.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqdiyzib.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xsrrqobj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3szpesynd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jnyhggxo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnphpwwy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3auzupxdd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lbnrklfb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dzoxzrpu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3msrruwmf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ewvnzpso.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3kbegwtoj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rvfrdqxt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3sdkftznw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jvytirxq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kfhoxvrp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3njzdhtyv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hitomlov.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3opeakhak.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3edfhtfxn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lqwgugiq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3xfxsmqje.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qrgbaybj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ambcnzug.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nnrevjyk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3cgdziyno.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iueghotg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3gaeolkry.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rfwggmam.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hhkteeyj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hjreisuo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vwjnqmpq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3thtgoeme.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vlfgbbwi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jhhyxgpo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3eoejugng.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3amizjsar.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bbvgcvca.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3cezxgqqi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ffjnvfgy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3xxveqqdl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ytambdzl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ginolusx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3klhzemte.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xsoewxwx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mxhhdgvd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3eybldgnz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vwfbqfeb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qqefvxun.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ngwadpce.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3lhbcpuih.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3sxqgnbtb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3qxviyiid.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ruxjlcrz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mexaimhr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ckteuwit.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wdmrfbdj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tuktljco.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3roxtwonp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3izboaigb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iuhuazsq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jhgrmyny.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vcgodqxu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3svuuxrbk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3kgpbtmxs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xkfclwqb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kxvuisnm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gspvukof.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vwxufitg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3hsciuqph.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mdxftavs.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hvfavbvk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gkomjnqp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3frbzetpm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpehtyyu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wnwyzhqu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wbebvfeh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ovaxftvx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3aremlaav.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fwlidnqh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kcdhcohs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cdovwanc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ealpbtyy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xcycorbj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rogrieyv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xgwywezu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vrgamcrp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lwbuknvv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3frtfbtap.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3joazqmnt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3lkhgzffg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3udzstwwh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cudhgspj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ewbxjfsp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mqedeovd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dkobphhe.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3duslnaxt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jdeylryw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ttkecltv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ofjficfl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gstxaozd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ifwnkghy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3umaoitxu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gdmkucnq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lljhnhdw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrbomll.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ymaapdee.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ixqfqowm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rqvtcrba.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fmtpekia.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cvobcela.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dpkqigsf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nfojxayt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tgxondpt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3wdwunsbn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vfjjlpge.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wsopcwci.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lzbhhmna.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3lnnllixm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guovrnie.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ogkvsavn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3xhqibdsa.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wzhfhsxu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3dettkzwn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3gkkcvyrb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3wkjvrodj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3yzlfebda.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ftsyyxnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieposjgv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3lftkczlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiebsqof.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3uytasfjs.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pludzbkj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gwfbknhn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mzysbund.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kaapscxk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sjhhmxow.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lzujbxcs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cglfpnte.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jfredrcv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ternhzhg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mfusdujc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3wipliuht.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mzalkcay.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xzhpzogg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gbyoihcp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ujzahaje.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lnrwnrok.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hrbaoesi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bjojorce.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zdndigde.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wbhvhsci.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xrvhxftt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yybnypaf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lgispuhn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uvtdabxt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3rsfzlnjl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ayflgghn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gzbwjqac.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dgybiwkf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cwemrxeq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3velkiemu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rzcwpwoo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3imfkwfai.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3llimorpg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3obxnxzsf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dkjthfjj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nqlqgusu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kpibtoqi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mnubhjle.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3fhpouymn.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3qefceftg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3xocjgryq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zecsxgct.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xcishxbd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ygkcrzsc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3slalklpt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3svyvfxuu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3cmcadcsl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3yrygkrvt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3kjwernvx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3xsyjivwb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3tzqzguld.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3baqagawp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acddmtfb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bunqjgot.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3rjwvmnbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmmuyttj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3bilylfzo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3moohsbss.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3qworqaov.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3osalxwvr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zuhdopjy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3btnqybzq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3xuslxlzw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3rwvuisfk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ehbssyob.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jygaslot.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3mukpmisn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3vgudbsyv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rfetmqan.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3oqahwrms.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ykvcsuor.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fktagyda.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3apiwtpke.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3aflqmrej.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bdvaifgc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3gxkevvtb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3umalxagf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3hfxtiary.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3revyvstp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jvttupbd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qsuckjae.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obutxzfn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jruwrvha.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fdbjrgzu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jenwnpki.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3flakkicn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qyddkolc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wlxrboan.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jxklstuv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mjmekqwe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kyvnvtnl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axmsngsu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3whxafrsu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3dnewnkes.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wilkgbat.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlwjgjek.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lybrhqyw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3qxugwxiz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dyzwehbt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ewbfaeis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqibpznc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vkgdnppm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyoosduu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3opcwctnd.html


<!-- 参考信息 -->