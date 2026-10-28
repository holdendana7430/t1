代发 wailian999

[U33] Py：打包发布
来源：http://hz.gaohongyu789.top/gtemlcytio.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gogol.net.cn/gtwfozesvx.html

[U34] Py：判断编码
来源：http://hz.yvedp.cn/gtezajqzos.html

chardet.detect(raw)
来源：http://hz.bjfxy.top/gtlddarksi.html

[U35] Py：发送邮件
来源：http://hz.xinyue.icu/gttmywdefm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cdnleiting.top/gtxzjxbkfh.html

[U36] Py：定时任务
来源：http://hz.zycfv.cn/gtykthnnoc.html

schedule.every(10).minutes.do(job)
来源：http://hz.hammf.cn/gtkvixozwo.html

[U37] Py：读写 Excel
来源：http://hz.xingfuxueyuan.xyz/gtdkhalnzt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.daria6918.cn/gtfqumognm.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenjidiqi.icu/gtqxltmkti.html

Path(__file__).resolve().parent
来源：http://hz.mhx1999.top/gtpsvrtumv.html

[U39] Py：判断是否在交互环境
来源：http://hz.smart0.xyz/gtxhukkonk.html

sys.stdout.isatty()
来源：http://hz.ywan-chungtsiang.top/gtbmieahse.html

[U40] Py：打印到标准错误
来源：http://hz.ywan-chungtsiang.top/gtsvhufvjq.html

print("err", file=sys.stderr)
来源：http://hz.feifeiyinyue.top/gtecnyvcya.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.0kj1m.cn/gtvzyrgmnp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jyoumei.cn/gtcpoenwxk.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gzhubu.top/gtlegrevhw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sysykeji.top/gtshlrcwzs.html

[U43] PHP：声明命名空间
来源：http://hz.shanyushiyangtech.top/gtntkhkgjq.html

namespace App\Http;
来源：http://hz.52xcode.cn/gtwhqrplya.html

[U44] PHP：开启严格类型
来源：http://hz.yj202588.top/gtijesoyin.html

declare(strict_types=1);
来源：http://hz.zycfv.cn/gtwynkejpj.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtrdviqvje.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtujgordpb.html

[U46] PHP：可空类型
来源：http://hz.hfpthk.cn/gtofgxmbpk.html

?string $name = null
来源：http://hz.iojbl.cn/gtwusnzkqx.html

[U47] PHP：联合类型
来源：http://hz.jinqigfzy.top/gtotgyxzbx.html

int|string $id
来源：http://hz.redwolf501.top/gtcylmfsjq.html

[U48] PHP：纯枚举
来源：http://hz.yanxiufei.cn/gtsouagqko.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhongyouzk.top/gtybkynjyh.html

[U49] PHP：只读属性
来源：http://hz.aibaodan.cn/gtpxybhtvi.html

public readonly string $name
来源：http://hz.shangyingyoupin.top/gtghohdybc.html

[U50] PHP：构造器属性提升
来源：http://hz.shuidangran.top/gtumeblosu.html

public function __construct(private int $id) {}
来源：http://hz.xinyue.icu/gtexzaoctl.html

[U51] PHP：数组解构
来源：http://hz.hfpthk.cn/gtvztqfkny.html

[$a, $b] = $arr;
来源：http://hz.jinqigfzy.top/gtyoafeklf.html

[U52] PHP：箭头函数
来源：http://hz.gotoacloud.top/gteqryyuqo.html

$double = fn($x) => $x * 2;
来源：http://hz.ppjwa.cn/gtqvsoblje.html

[U53] PHP：空合并运算符
来源：http://hz.jinyuanbaomall.cn/gtlghipmmn.html

$v = $a ?? $b ?? "default";
来源：http://hz.gotoacloud.top/gtzqsnwdls.html

[U54] PHP：空安全调用
来源：http://hz.xingfuxueyuan.xyz/gtrwmbuasc.html

$obj?->method()
来源：http://hz.shuidangran.top/gtfalotxxa.html

[U55] PHP：match 表达式
来源：http://hz.gogol.net.cn/gtzyiobmnp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xinyue.icu/gtfcgorvim.html

[U56] PHP：命名参数
来源：http://hz.316326.xyz/gtbkbntemp.html

f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtyfwwfzkk.html

[U57] PHP：字符串插值
来源：http://hz.gotoacloud.top/gtlihhvpae.html

"值: {$a}"
来源：http://hz.jqgufenzy.top/gtnbexvdwn.html

[U58] PHP：数组三件套
来源：http://hz.quarkkingdee.top/gtledgphpx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.52xcode.cn/gtviwwpthy.html

[U59] PHP：自定义排序
来源：http://hz.cdnleiting.top/gtcezwuopl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtfwuxkvse.html

[U60] PHP：JSON 编解码
来源：http://hz.yongpay.top/gtsgvhlcir.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.redwolf501.top/gtszsvfcti.html

[U61] PHP：正则
来源：http://hz.xingfuxueyuan.xyz/gthukdgtwj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtemdutumc.html

[U62] PHP：日期对象
来源：http://hz.sufxvd.cn/gtxuvklrlj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cheryme.top/gtleexssll.html

[U63] PHP：文件读写
来源：http://hz.9152youxi.cn/gtlsuhuitz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj202588.top/gtpehpvoaa.html

[U64] PHP：目录遍历
来源：http://hz.jinghuilouyu.cn/gttpkewhwc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hywenlv.cn/gtppllscrt.html

[U65] PHP：会话
来源：http://hz.meibo888.top/gtmbqtpsuk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xuetiantiany.cn/gtxnifepqu.html

[U66] PHP：设置 Cookie
来源：http://hz.hammf.cn/gtunfzscsz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnxiangtu.top/gtvrmvjnxt.html

[U67] PHP：处理文件上传
来源：http://hz.jinghuilouyu.cn/gtuwjrzdyx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ywan-chungtsiang.top/gtfiafrhhf.html

[U68] PHP：PDO 连接
来源：http://hz.xingfuxueyuan.xyz/gtvmtnelbz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yonumen.top/gtkgotcgqb.html

[U69] PHP：PDO 预处理
来源：http://hz.shzxlz.cn/gtleqbqlum.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tianlin.xyz/gtyiqkhfje.html

[U70] PHP：PDO 事务
来源：http://hz.shanyushiyangkeji.top/gtvwczfopl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zdqjudy.top/gtskvbltqk.html

[U71] PHP：抛出异常
来源：http://hz.dashuyun.cn/gtsmxpauhb.html

throw new RuntimeException("失败", 500);
来源：http://hz.wangdashe.top/gtipulpzqw.html

[U72] PHP：写错误日志
来源：http://hz.yongpay.top/gtatkhjzau.html

error_log("失败: " . $e->getMessage());
来源：http://hz.haohaochexian.top/gtzhatqrmn.html

[U73] PHP：读取 ini 配置
来源：http://hz.guowangkeji.top/gtctyyjvkt.html

parse_ini_file("config.ini", true)
来源：http://hz.jinyuanbaomall.cn/gtyrgwybmn.html

[U74] PHP：读取环境变量
来源：http://hz.jinghuilouyu.cn/gtsgilxasm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xinyue.icu/gtlgouxyek.html

[U75] PHP：依赖注入
来源：http://hz.aibaodan.cn/gtykbvlaot.html

composer require psr/container
来源：http://hz.wangshuangyany.cn/gtojmkscwq.html

[U76] PHP：简单路由
来源：http://hz.zdqjudy.top/gtvfnxrbaf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.andypj.xyz/gtsqcudllj.html

[U77] PHP：模板渲染
来源：http://hz.cheryme.top/gtejilzpvo.html

composer require twig/twig
来源：http://hz.gzhubu.top/gtxgwduzlr.html

[U78] PHP：单元测试
来源：http://hz.hysaishi.cn/gtibakvmpx.html

composer require --dev phpunit/phpunit
来源：http://hz.feifeiyinyue.top/gthectffnp.html

[U79] PHP：静态分析
来源：http://hz.xingfuxueyuan.xyz/gtdwuxhfoy.html

composer require --dev phpstan/phpstan
来源：http://hz.jinghuilouyu.cn/gtzwdmutvr.html

[U80] PHP：代码规范修复
来源：http://hz.ivvv.top/gtsjbipcoh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sxryk.cn/gtfljroghk.html

[U81] JS：初始化项目
来源：http://hz.dashuyun.cn/gtziezcfhz.html

npm init -y;  npm i express
来源：http://hz.zdqjudy.top/gtsajcordj.html

[U82] JS：package.json 脚本
来源：http://hz.fengsongda.top/gteetumltl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.andypj.xyz/gthiuprmwr.html

[U83] JS：ES Module 导入导出
来源：http://hz.yj20258888.top/gtzyxvziuf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ydjk.org.cn/gtwyvjndby.html

[U84] JS：CommonJS 写法
来源：http://hz.hfpthk.cn/gtixfdkbjo.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinqigufen.top/gtufqnuvht.html

[U85] JS：可选链
来源：http://hz.guowangkeji.top/gtnqgkpbzp.html

a?.b?.c
来源：http://hz.hfpthk.cn/gtisqovxho.html

[U86] JS：空值合并
来源：http://hz.chenjidiqi.icu/gtuwwglapq.html

a ?? b
来源：http://hz.jqgufenzy.top/gtnqmmlmqm.html

[U87] JS：解构默认值
来源：http://hz.xylfe.cn/gtnrcuszmf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.andypj.xyz/gtdfkzpoyd.html

[U88] JS：对象展开合并
来源：http://hz.shanyushiyangtech.top/gthekexknd.html

{ ...a, ...b }
来源：http://hz.aibaodan.cn/gtiywcneee.html

[U89] JS：数组去重
来源：http://hz.jianghu66.top/gttoqyedkb.html

[...new Set(arr)]
来源：http://hz.zhengqikj.top/gtxktoveaa.html

[U90] JS：数字数组排序
来源：http://hz.xinyue.icu/gthlceidaa.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtywtksozu.html

[U91] JS：对象键值遍历
来源：http://hz.sweek.top/gtppnjqlcs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.nanxuanxn.top/gtrxtutnwf.html

[U92] JS：深拷贝
来源：http://hz.hysaishi.cn/gtcgygndpw.html

structuredClone(obj)
来源：http://hz.52xcode.cn/gtkjvzzoqa.html

[U93] JS：模板字符串
来源：http://hz.xylfe.cn/gteridsngi.html

`共 ${n} 条`
来源：http://hz.cdnleiting.top/gteugknmth.html

[U94] JS：箭头函数
来源：http://hz.hnxiangtu.top/gtcedbhfhz.html

const double = x => x * 2;
来源：http://hz.yueranfly.top/gtpbemlsby.html

[U95] JS：Promise 包装
来源：http://hz.gogol.net.cn/gthojlfjml.html

new Promise((resolve, reject) => {})
来源：http://hz.daxiang520.top/gtzopucfyx.html

[U96] JS：async/await 与异常
来源：http://hz.shuidangran.top/gtdzyvadwe.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gtlzcabuaf.html

[U97] JS：并发请求
来源：http://hz.9152youxi.cn/gtlslzxeok.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtipvsugis.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gtqgtgfxij.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pycfn.com/gttrqlprqc.html

[U99] JS：事件监听
来源：http://hz.jinghuilouyu.cn/gtuyklfezm.html

el.addEventListener("click", e => {})
来源：http://hz.haohaochexian.top/gtvrzmfhcu.html

[U100] JS：DOM 查询
来源：http://hz.smart0.xyz/gtgzrepbzy.html

document.querySelector(".item")
来源：http://hz.jianghu66.top/gtmdguzocp.html

[U101] JS：classList 操作
来源：http://hz.xylfe.cn/gtsmrnvqlc.html

el.classList.toggle("active")
来源：http://hz.birdmap.top/gtvbeobnle.html

[U102] JS：本地存储
来源：http://hz.chenjidiqi.icu/gtgbeqpkqs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nwbrower.top/gtkdftodwt.html

[U103] JS：定时器
来源：http://hz.guannengcc.top/gtaxnblnot.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.wangshuangyany.cn/gtgoxjhwft.html

[U104] JS：防抖
来源：http://hz.52xcode.cn/gtunzvrqcy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtqowterhf.html

[U105] JS：节流
来源：http://hz.jinyuanbaomall.cn/gtwvwqnian.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhengqikj.top/gtfypouxwi.html

[U106] JS：日期格式化
来源：http://hz.jinghuilouyu.cn/gtimexqxnx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.chenzaomai.com/gtcwdhnrbn.html

[U107] JS：数字千分位
来源：http://hz.cucudq.cn/gtyectdfzs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.guannengcc.top/gtywnjpkyh.html

[U108] JS：随机整数
来源：http://hz.fzhhl.top/gtxdcobfll.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.quarkkingdee.top/gtexqxixys.html

[U109] JS：数组分组
来源：http://hz.jinqigufen.top/gtiwxxgjnm.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtwsznmhso.html

[U110] JS：数组分块
来源：http://hz.daxiang520.top/gtiuiboxyt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ybcxt.top/gtokwomcwe.html

[U111] JS：对象转 Map
来源：http://hz.gotoacloud.top/gtsfhfmlda.html

new Map(Object.entries(obj))
来源：http://hz.dashuyun.cn/gtxjznrrrw.html

[U112] JS：字符串补位
来源：http://hz.dianchejie.cn/gtlfblsmpf.html

"7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtsqmueuqw.html

[U113] JS：正则替换全部
来源：http://hz.hywenlv.cn/gtzsftezds.html

s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtqgdsodvr.html

[U114] JS：JSON 深比较
来源：http://hz.aizwys.cn/gtegphwjeq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtrmbpvbob.html

[U115] JS：生成 UUID
来源：http://hz.sufxvd.cn/gtaakvxyrt.html

crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtvllgeeom.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tianlin.xyz/gteolvzoqp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hongshengwenyu.top/gtekpuukmv.html

[U117] JS：单元测试
来源：http://hz.dashuyun.cn/gtqgafbqvv.html

npm i -D vitest;  npx vitest
来源：http://hz.9152youxi.cn/gtyhbzyqpf.html

[U118] JS：开发服务器
来源：http://hz.9152youxi.cn/gtgmllvcie.html

npm i -D vite;  npx vite
来源：http://hz.zhengqikj.top/gtgzvqzblw.html

[U119] JS：生产构建
来源：http://hz.yvedp.cn/gtbbexwmna.html

npx vite build
来源：http://hz.shanyushiyangkeji.top/gtzsbcybvo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.meibo888.top/gtulmluzow.html

import.meta.env.VITE_API_URL
来源：http://hz.shangyingyoupin.top/gtfufvcjuq.html

================================================================================
来源：http://hz.sysykeji.top/gtwleqskph.html

统计汇总
来源：http://hz.hysaishi.cn/gtvrpvgyoz.html

================================================================================
来源：http://hz.jlsjyb.cn/gtogfoqfdo.html

按语言统计（条）：
来源：http://hz.xylfe.cn/gtfbycwcyq.html

Python ......... 252
来源：http://hz.yonumen.top/gtnkshdzdo.html

PHP ............ 252
来源：http://hz.9152youxi.cn/gtshapgpvp.html

JavaScript ..... 252
来源：http://hz.nwbrower.top/gtsujjseps.html

TypeScript ..... 212
来源：http://hz.cashguo.top/gthwdzcgij.html

Java ........... 212
来源：http://hz.aibaodan.cn/gtbvjfhsgr.html

Go ............. 212
来源：http://hz.zhixingplan.top/gttsnamnmk.html

Ruby ........... 212
来源：http://hz.gaohongyu789.top/gtrsgiuczy.html

C# ............. 212
来源：http://hz.zdqjudy.top/gtctyvelkn.html

C .............. 30
来源：http://hz.havefunace.top/gthogtugtr.html

C++ ............ 30
来源：http://hz.sysykeji.top/gtwutnqexo.html

SQL ............ 90
来源：http://hz.yueranfly.top/gtprwpbtke.html

Bash ........... 80
来源：http://hz.jianghu66.top/gttzjiattd.html

Kotlin ......... 15
来源：http://hz.xingfuxueyuan.xyz/gtuitgqeue.html

Swift .......... 15
来源：http://hz.nwbrower.top/gtuaflqanj.html

Lua ............ 10
来源：http://hz.cheryme.top/gtylxdbzky.html

Perl ........... 10
来源：http://hz.jinyuanbaomall.cn/gtkfuoazlf.html

Scala .......... 10
来源：http://hz.jinghuilouyu.cn/gtqggxykxp.html

------------------------------------
来源：http://hz.zycfv.cn/gtvffjumyz.html

合计 ........... 2106 条
来源：http://hz.svipenyu.cn/gtnkscwfdm.html

按章节统计：
来源：http://hz.yanxiufei.cn/gtzlyfceyf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtesnnczvo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.snrcjt.cn/gtgnfxfxvp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zdqjudy.top/gtotsngigk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtgdmkdhzi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenjidiqi.icu/gtkjjnjuzg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtrhmejjrd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gthcyrnezi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.dashuyun.cn/gtcrtxyxoc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtzjbplsns.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shangyingyoupin.top/gtugdrwhwf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtcgfnvmdu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtjrikkgxn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtbujcqwxz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtvwxhrysc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hammf.cn/gturpewbah.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtehsyjfiu.html

Q SQL 专题                              90
来源：http://hz.iojbl.cn/gtwbniundo.html

R Bash 专题                             80
来源：http://hz.chenlongwang.top/gtlpwsafxg.html

S C / C++ 专题                          60
来源：http://hz.shangyingyoupin.top/gtowcleomv.html

T 其他语言补充                          60
来源：http://hz.316326.xyz/gtuescdwlj.html

U 高频实用片段                         120
来源：http://hz.sysykeji.top/gtpyfbhbbf.html

------------------------------------
来源：http://hz.jinqigfzy.top/gtqxpkyeld.html

合计                                  2106 条
来源：http://hz.fengsongda.top/gtshrmzold.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtroyideax.html

使用提醒
来源：http://hz.cucudq.cn/gtajdvccil.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtotsymqom.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhaomingkeji.xyz/gtrhggdhaz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.gaohongyu789.top/gtspsdnhti.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yongpay.top/gttomxxylt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.c1oappe.top/gtakecmazr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.daxiang520.top/gtqqnowfjq.html

—— 文件结束 ——
来源：http://hz.jqgfzy.top/gtljjegoii.html

================================================================================
来源：http://hz.aizwys.cn/gtbbeqlxdb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jiagoushi.top/gthssonbjv.html

Common Programming Examples Cheat Book
来源：http://hz.sweek.top/gtpgegdknq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtttgoipuh.html

【收录内容】
来源：http://hz.316326.xyz/gtfrrlprsj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.redwolf501.top/gtohyheoxq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jqgfzy.top/gtaehrmplt.html

SQL · Bash · C · C++
来源：http://hz.zhijiandao.cn/gtdjbbiair.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jyoumei.cn/gtibkkrhme.html

【使用说明】
来源：http://hz.yangfankeji.com/gtbbcuembv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yueranfly.top/gthucksnhf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.nanxinkj.top/gtuuglduss.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xinyue.icu/gthdcytenp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhengqikj.top/gttojdeokt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinqigufen.top/gtddmbippf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yuanzhike.top/gtkoblgcne.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sysykeji.top/gtjcoxrdgb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.andypj.xyz/gtzmdgabxp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hongshengwenyu.top/gtrsihhvzs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.nanxinkj.top/gtrfebklpw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gogol.net.cn/gtpvnaxego.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sxryk.cn/gtscgcbbhw.html

【文件统计】
来源：http://hz.xinyue.icu/gtecpkbszj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.wangdashe.top/gtfumqaqsk.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtlrlhepoo.html

目  录
来源：http://hz.yangfankeji.com/gtptaqilae.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gttyyrbein.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xuanzx.com/gtstdhyafc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.guowangkeji.top/gtjwmypyyy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.tian-w.cn/gthdusncgm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhiwuduotai.top/gtntyednrp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hfpthk.cn/gtumqrztwx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.bjfxy.top/gtfxehtqsp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj20258888.top/gtorvfbtqo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yuanzhike.top/gtjlvjllhg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtsrpmbdkm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yueranfly.top/gtwcegbqtf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtkydgcsrg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtjifbldfi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gtsokzsucv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xuanzx.com/gtlxznjkpx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.gaohongyu789.top/gtuazcfegr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtshlpwqiy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ydjk.org.cn/gteqpnwkqg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydzc1.top/gtxaqfnocw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.tian-w.cn/gtvwagzgps.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yvedp.cn/gtvcpouypu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hysaishi.cn/gtftxccojz.html

================================================================================
来源：http://hz.yuanzhike.top/gtxxdymect.html

A. 基础语法与类型
来源：http://hz.sysykeji.top/gtsgzvvrlr.html

================================================================================
来源：http://hz.bjfxy.top/gtruawhzzr.html

[A01] Hello World
来源：http://hz.xuetiantiany.cn/gtugvfaxbq.html

Py:   print("Hello, World!")
来源：http://hz.smart0.xyz/gtztxwvrln.html

PHP:  echo "Hello, World!";
来源：http://hz.nanxuanxn.top/gtbuhbixdl.html

JS:   console.log("Hello, World!");
来源：http://hz.aizwys.cn/gtkpsrrblz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.c1oappe.top/gtxmxttklu.html

Java: System.out.println("Hello, World!");
来源：http://hz.ydzc1.top/gtltbiusgt.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.nwbrower.top/gtdfzeclqu.html

Ruby: puts "Hello, World!"
来源：http://hz.xingfuxueyuan.xyz/gtbqpfxjcw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hywenlv.cn/gtukcdgvus.html

[A02] 变量声明与赋值
来源：http://hz.tanke756.top/gtxdzbmkwd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.smart0.xyz/gtzlzrulob.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.haohaochexian.top/gtraaexhio.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenzaomai.com/gtvugonwdh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xylfe.cn/gtaukdybpf.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.pycfn.com/gtsqmrurox.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhiwuduotai.top/gtnuvxpaah.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhiwuduotai.top/gtpvsulgjs.html


<!-- 参考信息 -->