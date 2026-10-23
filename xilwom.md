代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zggugjjz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xwzjqydd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zxfzjftm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3oxnhjopd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3iydtnlii.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ntccfnlu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3hqtsvoka.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pmsdfbkh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3njixglxj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3zfyusvfe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tehqcsxd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vaiuiari.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ezpegijp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3hubfkgmh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vhbngnvu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3isvjshpw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3oiuohrmj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vtbkmoyr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hpwwlzke.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nvdazpnu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3luzjfqif.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3juwftphf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uceppqke.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3rngxokkl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nbqmpvzc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3tkfryeuk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kmgvwsyc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3cikizjvv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3agykvoph.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3payekogx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3mywgaesi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uhfrnpzg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vfiwyzdc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ampqsiek.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3scwpqixw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3lczdxrzv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3atvdunqr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3tqwmwckz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3sldrtzjq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3saywbunf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mgqluvqy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrjzjlsv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ozwjskba.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ahkhmxvo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kwqqdlrn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3hvfngegu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aakcuapo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwzamueu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hfuwdihs.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3btavbzqc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wxedvojc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3orrroosr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3glomtxdy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ncglxquv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvppiddg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kuiynsbo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3uinyyvey.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hgricqxf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3yubxtbcg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fclootmn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qfotqtik.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zlflxdfq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3tzxbonhh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3envoexit.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ygbzatfs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wpmfoxwi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3dcsbvxlj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ydxvuaoq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lmufeqlk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fbeelmxk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rercmnwh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jmbayady.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gomgzcos.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hnnwlffr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3shwuedrg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tyxeueyg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3steoiezw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wlaquxif.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ubugmehf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3eejbjugb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3deoqxtzz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ybnpgjsz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ogcefcpe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dpxdvhwn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3onilbncq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ljqkjufb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qtjifyqb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3btmdkdzm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3betziqro.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bprfzjuj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nqfpubqm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sswucilq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vizrljdt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ndfwsjyn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3rrkykjfb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3fkqfhcsd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3mevjvqat.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ufftgtzz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cqcefcbd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qmzehfsm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jdyjlxsw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fkjxhtvi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rplmwtwu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3venkbtus.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3kauzufyn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3eyftnqom.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xgsxqhfk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3okgjcatk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3spoflvuy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fletwfii.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vfrjjjlv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ahmlgtxk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3piqutpjc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3uzrjfegg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ssbytzck.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vwtmbxdw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3oqguapeo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cncrpvjt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3oguuipyb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3lqhhtqmx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jtjhpzgq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hfxklzea.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vwhoukaa.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vtnezqdp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3kpafsdpl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vxrzeifc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gxhoyyvn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tzmsrwyb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xekzfzxg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lbjnaeii.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jmjermxo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ljsecwpi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kfhraebf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ffjthjdv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3awyeacdb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdpzhmb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zvyskxrb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ahcruewu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3roidahbl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bucshafu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3lrezprwn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sbgujjvt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3juzlemhm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3brchmdhh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3rsrjkpjg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vgajhwbd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vhkkkwtt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ojhovbni.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fnbgdxru.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pfterccw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bkgwzgla.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3alvzlqbd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3rqbtdfip.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nahrqknq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3najyvgse.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gphdomuu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jntyhjrc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3luurohcq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3recjpvny.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bjtqrovv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qqzurkux.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gtehuoaf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qtgwvboe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3hysotiss.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hiuxpezc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3imtgormz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3acyfykjx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gexezsyz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rahmqyrg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bzrvegbj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bmyftaij.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dqlefpii.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3acceutno.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lctqpgkx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3okqlttgh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dsxcjhcg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ygrcgzln.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lrnwizrj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ybzrhzrr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rmmfyfmy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ctrgpjgs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uekewawj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ydxkbxms.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qonmzkix.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pazaxzpm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3tlxoksbb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wkamgwof.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3bdrbgska.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kgsycsbe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ytteazug.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3lnwzwudg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3lbhulnuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqltsdhj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gndmjzbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfjzvkuh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3bkgnswdv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tefdjfhl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3lxhzushx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ftzoyftb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bsoiswem.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pwknoqxs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wsrlsdey.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dgkzdovl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3awsfxklg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3wmhbbutx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mgeknmjw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mvomdido.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3iuibkhfl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zrzpflsq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3uekvgymp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xclnttei.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vmkraslx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ritwbmii.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uwfihjhg.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ejyybhoy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ajlymxhl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tngrvkvh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tibcbifs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jkcrzzfx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rsotquvs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3pfbflssf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qjchgjxi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3adjrectk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3znadyrne.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ujsiowei.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dlrtqcnl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xualqvng.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vrnwnsns.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qyjegijr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3froboqpz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3pcmkwbdk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ynxgrycw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3xqroqudb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3oxbekevw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3mfqlimjn.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3zncarowk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3mwhrgoih.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bhuivqoy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kazeuxbj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gboqktvm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3awbujjiq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ggiahhqd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xjwcewiw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3oddvzqwz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3etvnmojz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jvfurbjo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3zyttcatj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ztxmbxbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddybdqjy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3jtgfuqxk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3fsxsgkdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxaxmxdu.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3nqgcsitt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3djkuflry.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cubouefr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3edgstrcd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ogdilgfj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3htchqcsp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hdjjaaeu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3pcmtmkfj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3gtbmodjg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3qhovgkun.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3zeocfnvj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3gbpzjnik.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3cijtdvnd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3euprnwgj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3unisfzkd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3bzioqwrc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3gxsdpyxv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3rczbckvd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3opdtceza.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ajwqwdey.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wrxdcfvi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3kcobmpfo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pgbjsvmx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ygxqsxjt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3coyulpbr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ypyknied.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ezxysfvr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mfyaimup.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wpwtirpt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3motjlgak.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iqhxmkyj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dnyirrdr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dnlplcvs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rmbvobqu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kflucygw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iygtzksf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xwgbmdqc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3eukpkiwg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rqaokzta.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ikadmiyp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3phbyoxlr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3opeznrdk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wkzvohyd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tkfxshaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkxxgirz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3esikkaip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3biglvxku.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xkhncavz.html


<!-- 参考信息 -->