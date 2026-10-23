代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rzxwrsfw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3prwapsyy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3inxfswzk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lvdkxart.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3seviwmte.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zyukktdh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qsorbihn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3wbouprkt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3wejlicoa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3jbvuigmk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cikuphld.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ugkopzhl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3duyvyzac.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vpbqmlbc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yhwsgjez.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mycbbtid.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jrxwkomt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3nkgmralh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cyxecvic.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xbqottfg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3aizpgqwa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rbxfwvde.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3esmlxrja.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ffrlgdws.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rrakypry.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vibxfvum.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3flbkpyzz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3cobuctxj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3fxfzkzvq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3lbvmbfsr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hiczvixv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3rzgdmumc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3axbkhahg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zfjfbbtb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ptpspsma.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fflgengh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3smjajfwj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3serzdfve.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vqhllmvs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3staecabc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yshnvuod.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cqawamge.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ueexvrqv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nhyihngy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3mheantlh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnshohas.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3fttplnem.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3djvpuwlk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vzxywdym.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3togbjpwb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3onylwkwz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkaapyca.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3iebvfylg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3uejpzzxz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nyupbmpw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufvqlsaz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3luskmekt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3pwfovvyn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eyvvumjr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jtlfsshi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fxyggqia.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3uxegfrjg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3kzkxevow.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jyvcpyqo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dwfdwjto.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gxfxekzx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dwfaqexq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhrynhwh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zzjmiqka.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3nencdcwn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3alssnuxi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xilwzfpu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zyjjlvsp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dcbgzrjh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3zpeyozpv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vbflistc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3pkgokvgi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qpjgaxfv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jhswywye.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vasgcxok.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rlyvhohz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xzqgrvxd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ybwzicge.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wpufqoli.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vkzfkgvy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3snstkzmy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3aglzydtg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hwjwruye.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kvtpndnq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tujncryj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3avsulgft.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jncdenhe.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3uebnbmtc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3brwsbeit.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zqapvbut.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3nuixgohx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lxyioryv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3euqzqsvt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3uenhzlvz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3yepguoqz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dqjzudse.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3eiohburi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ofzextaa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lbhngcma.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hipugnxi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3czlocrvv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qcdsfmxs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pbhfrshi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3mtnejzjd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ktuckifx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wangbbqw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3weoaczkw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fvjlhoce.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zctzqpfq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3msbocjww.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bhskrfmf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3cnalaphg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hxejekjv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ksjzbkgr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ewsbuojb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ddocakph.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vzjxrcry.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3swpdepwx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ehcluyhl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3dsrlmkni.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gmzilish.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ktjcipts.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3afxwrubj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yabwsiqp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dsorjqkn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dbvozjvv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bintfjhm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wwobsrxl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xotzdgng.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xavrklal.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kzkflphg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ooposvny.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3fzmlkiay.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gyzdaoyb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3affrsoiz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umjgtebz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gzilkziu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qicbquzu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ovxnaseh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zkywcznd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3egmeghvj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tdfgmjns.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygafbqll.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3rdrzetyf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lofpigyq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qgkxqvbt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vhiskjbu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ikxqyifs.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lohookmt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3muiudtjf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tuujylwg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3hbpfvwbn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ujlxcxpn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3macdaugx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dinfakrc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ufldiszp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pveilvbr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3cbwxzkio.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fxmlcrcl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3uznijezm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3kjdeffqy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ojvnzjxm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3trkqbmll.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pcmohzxk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ivakslvj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3frezacnv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qidbvhfu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3uxtcwyhm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wnfbffcw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qycxbcyi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lvhktucc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jvizfvtj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dqxakhng.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3pkxxmzmj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aitfujig.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dyzfdvyz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ynryscqx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3dtazuulm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bjmnfzep.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ivgjdjub.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iyisybio.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3uuayuryu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qakgtwif.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zdhwqfts.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3omczefuz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mxtoyzjx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3cjswejac.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pxjhmfse.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qfizayhs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3cfbsrwae.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kxszdfzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yedvnfye.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3cnjprbou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mitckqfj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3grwupwls.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3okvfgzek.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jutejkks.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lzwaxzzl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xowlyvvy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qotsddlw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xvegbkkg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mwnqefgr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mongmbhy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gargbpxb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hunyewfe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bxstraql.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wpkmllib.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wrsgsxee.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3pasdwtfj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dnqdjajs.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rajufjrg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rkmlljtb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gfrshmyk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uwutosyf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3lohmwdmp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qijixcal.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sbubvucn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nnsvazks.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jabanrgx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3secynqlr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ufntsrmj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3niowkwyj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kbxoyzol.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dlqcwhpp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sjjivdzr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vddmwptv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fxfopibz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bdmsleip.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xercraws.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3anzioscs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ozwgwked.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3wpjpgfro.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3vbyohcjv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3vpbshkpx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3gwotronp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zxlqsycw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3abjwkbam.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3imnhvluq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fzsjhalt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xtnymfdi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ozetfaaj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3clcqdwkc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3mjjoosik.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3vivnbueq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mhbtzjll.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jdmppjob.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xxrucsvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqbkeigh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ttgdjguv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ndsecqxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yurbsrxf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3hakuzvyy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qwdjfgsn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zgqyvzuv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ddcluuqk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3xcknsoss.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3cbezvryj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3gedptwzd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3prrqdrdm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3wweyxupn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3uczkqhjm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ifaqgtji.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dfambldu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3flgxvcoa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ustzqhcw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3axprzlef.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gwtyyobd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3okeoikzp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3rjuvhdeu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3gxbkhgwb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3gvxxzhki.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aaiutefm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3scqwqnjm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zpjofjug.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ffijzzdu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tsitjtrn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tnrptcxx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylhtwhvs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cergatmr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3aqibhufa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3idrldsot.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ufggdqnt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hhuekoys.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lgnnayuy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dvvhtpue.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fqnkdctt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3exvzenql.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mmreslgy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cflilmnw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ekzfkarv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kciagjes.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ojcwqwco.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bjdqxzsm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rbtiopnb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3osxbiyse.html


<!-- 参考信息 -->