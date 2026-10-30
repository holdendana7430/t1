代发 wailian999

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gycdarehm.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gvrkpckun.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gqpaesyvq.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gmmdbdoin.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/ghkjyjlby.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gqpihvakp.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gjaimtvfs.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gxouoiptu.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/golvjdqlb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gdazpoygv.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gmfapqjsw.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/givwfodrh.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gnybbzpjd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gnhuwfvnj.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gtuuxbunt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gxgnjshek.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gkcexyyky.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/giznheswo.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gqmswwfca.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gyxlurxvv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/geeygcvrx.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/grvjyzfit.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gctiuinlq.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gymsulgwa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/garyrloyw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gxiihsmxb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gezczfgiq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gtxrrocbi.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gskvuvzsa.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gxnfqjvit.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gucvrmuxp.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gsqkzzzfb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gmbuqotit.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gocizklon.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gswxtzchu.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gcqshbzli.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gonzzyixq.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gnpyfyssi.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gxcnastdq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gqzfmbopo.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gbrakcmiw.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gwwbtlodo.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gywulwwrj.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gtiimhptt.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gdzuvrdcl.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gneoebqno.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/goxatvyli.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gloofrrbt.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gikruchwv.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gvkxcazgk.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gxiwrsypx.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gpnzujrbj.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gouunqgte.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gjzcmvhjd.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gqhpfwtqs.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ggxbgvgsy.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/glmmlzwcr.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/glmaqeqqc.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gulsbwwsh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gropktdyg.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gyenbtnrl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gobgdhiye.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gozobulif.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gnohqivga.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnvonai.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjwdmymzf.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gurmmjmpa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gimvmndbs.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gehezgkfj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gnolyxhvh.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gofmqaevh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gxojtxswx.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gmbodqghs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/girofpsix.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gqvgxbhqw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gcvsndiuu.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gquvdbelq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gefqegfwu.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gknlwuwkh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gqfieopjc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gkfvutdns.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfzcglccb.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gexseeqev.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/ggqtkgkfa.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gwktcwoqm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gzzyhhpit.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/grkqbchdw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/ggcmuezhb.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gumnbinnj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gyxokjsxk.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/ghetxysdk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gkyssrjoy.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gvvwctobz.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/ghnntnvmv.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gsgdjubpm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gzxckqiov.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gqpfdrrhs.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gokujvkrn.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gbeesesan.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gnexqbfus.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gqvfymcoz.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/giuwdetxv.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gabjfcaxb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gmbytsgdc.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gtjmxbtii.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gzlmvxydd.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/ggcewzuvs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/glfzftkkr.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gbggvanig.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gughhqvzd.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gcyseryip.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/goamkfmrh.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gekzmgcms.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gtyvdkjim.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/ggalgmxux.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gynquguuu.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gtnottkgx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gcigdnlgz.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gpjftsawt.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gluedappo.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkybkgw.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gsfjwgffq.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gcemrppel.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gegwshtwf.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gaiovfczi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gkadojyva.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gatljwnjj.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/guhkjlfpu.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/geerhatcd.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gcjviovgf.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gktzaparo.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/ghvhbihnm.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gvhsswigk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gkwscovcf.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gzmasdlud.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ggmciozal.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/govumgcli.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gnknvjlmo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gkxxwmivr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gmhngrchl.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gculauzze.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gbitrxstg.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gosmojxjo.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gulrnzkyf.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gizlmecso.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gxrkdwoqo.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gcscuvbpq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gkwhfdtwx.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gsguqermn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/guppihtti.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/ghjfcfonw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ghlgxmtkk.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gispfwxch.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gkdrkyjqa.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gnuvgyftq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gfierqnpk.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gwdoyusrl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/ghwaduobr.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/ghzqlgyok.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gbzxvdrnf.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gjozhjvvh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/guimaklvq.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/geemmpwuo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gufdytiax.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gkcxvygmz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/grvqdcgeh.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gzyuolufn.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtcupfsst.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gdnckxfye.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvperdspw.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gnkvwiplr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/glpmypshi.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/ghttfsfpw.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gpchkzjvi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gxfjvawsj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/goknlpbmq.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/goajilprs.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gmrchoezu.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gryllxbxe.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/goyvnbfpb.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gcrdtkvkq.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gqdqrjwpx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gtxzrsqbb.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gqfjbqved.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbeulebuw.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gaidhqxbs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdwjbfixo.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gwfckhhvi.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/goqssrpxc.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gvwxtbsep.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gddfpxqzi.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gqisigdfc.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gstyjyqit.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/glpmkvzfm.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gyenepvty.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gllrapnbt.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gudgpdxpo.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gazvrnubj.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gtctpevvb.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gvopdmwvd.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gqockjdbl.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gxpzbbmmh.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gdwfokjok.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gacegjygs.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gyseegbnk.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gjimsxjze.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/guebxdyvl.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/ghzugcapd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gzbyebnli.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gkbgjppav.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gbtklikyd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/glanvbayk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gwvhlvshr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gvoyyhkhg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gqhncnkmm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/guxospqgd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gnntuybop.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gyzbotvab.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gqfhilycg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/grilynbqb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gngjgfulc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gmqtwtgug.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gvzngkuvh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gkjmlrffl.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gwcamgcbb.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gfctmfove.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gwzuohhsh.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gevohapqs.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/ggnzmbwfh.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gnaeikrdg.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gadaztcdm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gjumfihqx.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gpkaadcra.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gjuqozzwf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/goirnowzv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/geqsyfbdu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/ghjszotuw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gptspapcq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gstzbkygk.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gdtmbsmkq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gynpuvljm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gjhotxzzk.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gxkshitei.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwuuazaij.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gwpkbtace.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gxcchzbni.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gzevdusjo.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gpxqnpucs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gjmszjhtv.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gyffidrxc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gjypsgjbc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gcdvbamwp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gokctgjfb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gvphnuoge.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gxalugujn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gquagykgp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gaohoxfwd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gtudfczjd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gfyvpnewk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gpkubxbsd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gqwbjeocm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/ghnaitjul.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/glmoagayu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/ghamgzrye.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gaukjhsvt.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gdiasjtkl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gpwbkmvly.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/goinlhgzi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gtezwqooi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtnzbshak.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gbuwlgsaz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzgjrsyxg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gsqntqakv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gzpqpjokq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gmuyktrnu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gwpojvcqr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/ggijakvmn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ghpxrmspi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gadrzdfcb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gfinjhspu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gxyoveewg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gvfxdpruk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gjbiahrgf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/geufhzaaa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/ggceuzvco.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gwnhhckny.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gcjwqpbug.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gqfuacukt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gklgcamul.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gfozeramp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwtaijejg.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfddjsfuf.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/glybeqnql.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/guaypczos.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gghrhfbdj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gvrbhkucb.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/glusjrwfk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gxflvaqxl.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gjrgtvlwq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/glfhomdjs.sHtML


<!-- 参考信息 -->