代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zciyuyjf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zivpwqri.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tufpwamh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cercvzfa.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2shtdhdzf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bbbrmxsq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xesrwkwr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2eblptvvw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xydmoryk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vkyjcosz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2anwtbydv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2bcdsaiyi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2erfbmjwv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kjwtoyqj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lopoajwy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2skojkuru.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2kmpxyfbp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tbtihskj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rebyeroo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fabcxpki.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2elwitxdf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tlutmpwq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2beaynyww.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2sjsblwbf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ziqwdydu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lrifuqdq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2unheomoh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2hegcotjy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2aoyziczq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nfqdyjww.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cvllxlnh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2apddqllc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sopszyps.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2asljxmmv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gpamfdua.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mypopjtt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2poxrvthp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hznwvuza.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ueviejlu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vkolipwi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2npnggflt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tpnndixe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2woduypce.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gsbmvgyl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2aqcefrez.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2vdxuzxvm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2btzrgdev.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yxfxhkya.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ucuwfrnz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ggdvodik.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ggnzjfld.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uhldgctn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mtzxspee.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2odduepsl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ryhdzzfb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2uqooespk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dcvstmba.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uiuriyjh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2viqftplx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2idascyym.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2fnlrlvzk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2arhsugje.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xzjmzcqw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2hbsysphw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bzwhitiu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ifhippdc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uvlrkesv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2exkecoub.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ylkfpegw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2blbcstud.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jnzktgnz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zbmsuztn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2plojmhdz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2irustfyj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mpsnkxlx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2odskmkib.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2suyiwaoh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uelptvll.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2lybylkcr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vkeoebfw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qfurfjzj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xebqcsvm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zkqtjihi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2threskqj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2fwwydvry.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pcglqigi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zghzniav.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2fbigcnsq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qmdphaon.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nignntih.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ydwrgsin.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xtbhqppw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2eldajvvt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2uzarvqfk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oqcgzhgj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2auyuihtt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bjkvmolu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ognuccrv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lckmdeys.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2kucycbzb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xpnpbdab.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2tcwbsdla.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nhclcbwl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nhevaknx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tuaxikbv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gkwudpcn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ngtpnohr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jhnvuvmp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rvhtyzsd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2slhgztku.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kllgtlcz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2myaaqzpx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ccnersol.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2behbvdaq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2icnldalq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2enntgtzk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2rxwhhebe.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tmyhszas.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nxqzdwwq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ufpeuyvs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2iivamvsx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bbpdqouq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yqzcfxhk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2khsgwhhk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxlczbvx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2oklimrrh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xvkmyffj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2acfqjhiq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2tfvqytty.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bbgpeunk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vdkcpotn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kzgdfohz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2vhqhzkxx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vkeorfzg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mwinrzao.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2lowsmjld.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bsswmynm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wdggyyqc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2iwcayfuc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zwnedxqk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2anjhqgoi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2axasinbs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2muxrxlht.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2koptmkpx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ggsdamdc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nfcslymt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2aeaompia.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rxupbsww.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2iijpjqhc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ogpsfarl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2prmnllac.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2frmfcmlq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sydxofrv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nnjduujc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2cktfacsh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fanaljmr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jbqvlgqf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xsabcgnz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tutiwbsg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bfnoaeoq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xyxdkqhw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tfclbdwe.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2debxhuuc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kjecgdib.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2bcryfzff.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qnebfeip.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jhwozbys.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tbbmlunn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uccrkuhh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2amwtrufd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2cejpqfly.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2pspmrfvf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ufoihiuo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jvlwgxeo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zvlshjbl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wxbreqsq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2vyhgqehe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2htqvvvzu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jjtisuaz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mlucihyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsthnvxv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2sckcjmug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pneomaen.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2dqezhttu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nkxyohed.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2wfjtkwco.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vlimhwkv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tvtcoihu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rdsticsf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xqjqqkjn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fbbfewmw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gsrzfaod.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2igbgcqvh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2kioqjdzl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2bryjcnnk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xwpglrhs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2yfgfnqjb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2eiblqkdi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2sfumtklp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2rjghdqbi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vslawqrm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ntgnykcd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2pklhjquy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ucuzqhpo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2spsmpeji.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bsintkso.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mpmlfpht.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qqjngkqs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dgijlsef.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2irnegwja.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xufwcfbm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qexvkexc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rkgwqoel.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tofsxzrx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zqtkhysf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2glsrceuk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2brvvykmp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yxuvmmxu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2itpliiow.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zewuujvz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2evhukrvx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2vvhtzysg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2sfrzqshw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kxnfupth.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2yjpdwhau.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kbvmgpac.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2sxangljs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wpknierk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2yhozajca.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2quqqsrau.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2gypjqkzv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vsuebdyo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2eovqnali.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2tumbdaha.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wkvmeodz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ouodybqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdgvvdvu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2hgmueppv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gnlqaqpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcxhweon.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2amhsonfz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ondvqyff.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2gvthpcpp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jtvmsmcu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2mkpsjqdi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2gcwkwurs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ppvxtpct.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ivppvdsw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2cibwoavu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2dblkoecq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jhykpdwt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2zmxvkljs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2dzuhpaqt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2aryicktu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2sbyrronv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ocrupveb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ilwflttt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2gttrelmb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2xnyfbofh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qwmazqwu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gsjollwe.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2cxpbgwzp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hpiahkcg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nuskhega.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ezrbeksh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kvvxzsrt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2klybhecf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gtwcwyga.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bhseyqsw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dajpgkfw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvunzevo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ueabnxnx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qsgvbxii.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2etmtzgta.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2knsiyico.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iflugoaw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ulrvjukd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pokkvqva.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ycvaubem.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iqbdwiyw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wbwnjhdq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2smfygfyg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nglrpyhw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kmjtjdfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utxdsefc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2zjpstyrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cuhuskpx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2lpzhwuwa.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rnrgnegl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2fdqphymt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pckjryes.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2eludbhsh.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mysigaim.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2khldtlma.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hkcujued.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ndkmcybe.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lylrrpli.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2sqlafpqu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2amljryet.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ompbkknn.html


<!-- 参考信息 -->