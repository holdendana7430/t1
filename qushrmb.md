代发 wailian999

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gpkzpzeba.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/grfookksv.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gjpphkewo.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gqbzkcsui.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gjmvmiksp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gmmkbfokf.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gitaymwus.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gmllgqqri.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gsmgdaqdt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gqrcidtqm.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gqepubrjy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gqjcchxfu.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gdjeuiamg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gfrfxzisa.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gqlstqjsp.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gylurplya.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gmfdzjlnt.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gplenzpuc.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gnkezrlit.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gqdtcvhjp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gtxazyfvs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/guklddpxh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gtinoloot.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gsftgnluo.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/giykpzkmy.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gxdkxtdhq.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/ghzbibhvq.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gxkpkqtjo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gcxcbnugb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gmrqqbnll.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gcddshvot.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtfkqpd.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gnxovqtxe.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gymdiybns.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/geuvrwbds.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxefsgxz.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/giegzfrde.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/geieycium.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gyspxaiin.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gpyjmyckm.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gfmvzlefy.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gzplpxboi.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gvmcqfrxz.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gxchxtlva.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gtsepxmgk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/grsvesrnh.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/ghhqgsxmz.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gmwyzllbk.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gydqqxmhw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gttsxetaj.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gknzfqusm.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gmwtbrgsb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ggcpkqqbv.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gjjwvxeem.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gxqnzcmuf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gusoppfhs.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gvdjxybyg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gfmqbovug.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgttydn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/giktqqsuv.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gcoqbdjvf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/guanfkmoo.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gaiqyhojp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gqshvrsqb.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gyaqnswjg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gbpiuwnut.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdhawnjvs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/ghsqlxgzz.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gzsykqlji.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gasxvfqwo.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gwjggidoz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/giiksdwlf.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gambfncmk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gjiinpnki.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gtdjywupj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/ghzdhdexe.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gtkgbcrho.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gvylrkobg.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gjfocpmrj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/grmuzzect.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gklfudoll.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gpvretxmt.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gcobmkijl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gjoxxqzgd.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gkipvarrz.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gzkjoedid.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/geteddsiv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gylkmrkxs.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gsrdxntwi.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/guvabdull.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gjvwjwyqh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gkvcdfodv.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gekbsgxll.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gerbbeanj.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gfifjvkct.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/guakemqwt.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gubdthksz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gffitzqgj.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gnnprxbkw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gymsedgmk.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gqobbfkzm.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gqvhojilk.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gqwmhmygo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gfyzgrmue.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gokwjpjrm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gjfxqhygj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gpqbvblru.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/goilljkbz.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gsqjhssyu.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/geytddwab.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gcnmzkjnk.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gijwkzimj.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gwrybspic.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gkkwxyizm.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gtlwtrksf.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gegfrwxdt.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gnmnnsozg.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gbybhdrxj.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gqvegkgnf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gpiwvrwtw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/guanaltyg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gbvqcushf.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gvopbohqo.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gaoybblax.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/ghwvdndmd.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gxmkysdcq.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gnwfatpvz.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gqxuavyps.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gbavvxtho.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gqzdlgazf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/ggclpsmls.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gjyaplzzm.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gakjpwumq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gbwiqacbd.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gpmqfprho.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gwefjsuza.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gokipqosb.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gshllwvkk.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gfiodbrmm.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gmdsprdrv.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gclvnhszu.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gzbsygcwa.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gibyvvorm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gaschlyqb.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/geottnfex.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gwwjbigvs.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/geiofzwpv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gcrhjtshf.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/ghmbjfjwa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gvbcplmze.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gslpjxhga.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gdrniznzx.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gxvojlxkm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/grxgctbqh.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gpdlkofxl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gkmdyrumn.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/ggnfasity.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gkpzcocqq.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gxcvdffpl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gafacaxok.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gxxakjqfm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gorkkqtfm.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gewyjszce.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gnnegiiel.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gpdcapwei.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/giveutgzt.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gfhhixlsc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gxyzqibzu.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gutyizpaq.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gzkvcpdog.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gxhpsdxoe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/giazpituw.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gbrzarwxo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/ggnyxoeia.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gitnsrazi.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/grzvzmwyt.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gsgqiculn.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gunqqjkdr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gzpayonbr.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gwbteuxmb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggyapromr.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gnjjbpwpu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gojbqqxcq.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gkfqpkjji.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gdjvkyipd.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/griisfzzm.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gawhpsxdn.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gfoezjqgk.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gyrzdyifq.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gywyzkdio.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gvsbtgatg.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gpnqjbfxx.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gpoifuqxb.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gkehjhkgu.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gjkjomjak.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gmhmmlaok.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gkauimmyn.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gtxtjhbkx.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gqbamlsyf.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gsznqnxgp.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/ggfqsqika.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gbdglqtbj.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/giognctal.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gjwgzpjud.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/ghyltvxlg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gjcepdrqv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gxyfuncdr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gpeebemdx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gkhjhdcvf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gyebmoqls.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gbtbznqzk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gtkbbxloh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gqxnkknxm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gufclzzyb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gntgouodk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/glbmcqnui.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwpumdhin.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gigvzfiqo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/glbrdvvhs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gwoiwlfwp.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gpkigopci.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gjotzahsq.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gbmykvzah.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gzrpmjqvj.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/ghygtzmrs.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/godzyvnwu.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/golhhbkub.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gidgrailt.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gkifhkxoo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gzpkkbvaj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gqgriiekq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gxbousapc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gyegkewvu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gznabkabm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gdokbqtoq.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gotktzyuy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtqsbqwyw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/galiqvbla.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gqysirhku.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyxhyqalm.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gtnuzhffa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gesilqncr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/grqyzsomf.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gyqrvzngu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gpcdfnchu.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/groftkrxe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/glfatjvjl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gfgmcwsfl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gofuxxgtu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gmcgvfirk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gcdtprrzt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/giuaxfhnt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gxalrvqqe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gugfrbyrk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gpzxukpyv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gxldvwlos.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gnmipbfun.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gbwbcmhpr.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gnausjkny.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gsvdyphjl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gthndyaqk.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gczyqbriv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gmbkydpfv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gzfveyqwa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gkzbmkher.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gjliuavxj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gcqjrponp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjrapkvib.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gcjuivwst.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gadksooru.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/guohtptuo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gpnabfnpx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gskhvbfpv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gilmdsyii.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gyrojmdey.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gvudqehwh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gcooedbow.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggqebcdyi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ggzodhker.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gybiadopw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gqarvxglq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/glwpzrbqe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gazgnrkzb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxinkyhqf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gabrjewmd.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gfpwpkpvb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grbgrilrk.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gyluqtziq.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gwytspbhl.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/getwrxpqk.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gvabrlwjn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gxlgmtwqm.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/goelqnkwu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gxeborilu.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gzxfqgkhx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gvmujtljg.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gbrjziqnk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gzagaranl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gwhbdxwcl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gkyfxthhg.sHtML


<!-- 参考信息 -->