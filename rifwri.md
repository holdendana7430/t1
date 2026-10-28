代发 wailian999

[U29] Py：属性校验
来源：http://hz.jqgufenzy.top/gtradmbmiv.html

@property 与 @x.setter 配合
来源：http://hz.zhongyouzk.top/gtavjrsvin.html

[U30] Py：数据类
来源：http://hz.gzhubu.top/gtnzaqotvp.html

@dataclass(slots=True)
来源：http://hz.gaohongyu789.top/gtjqwevpir.html

[U31] Py：单测
来源：http://hz.gotoacloud.top/gtnmkefzms.html

python -m pytest -q
来源：http://hz.cqqwz.cn/gtcgcuqxph.html

[U32] Py：代码格式化
来源：http://hz.gotoacloud.top/gttasuwqda.html

ruff format . && ruff check --fix .
来源：http://hz.zhiwuduotai.top/gtrwcbovkq.html

[U33] Py：打包发布
来源：http://hz.nanxinkj.top/gtyiooyzxg.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shangyingyoupin.top/gtpygxptpr.html

[U34] Py：判断编码
来源：http://hz.yuanzhike.top/gtyqoiivwh.html

chardet.detect(raw)
来源：http://hz.shanyushiyangkeji.top/gtfoxspnwq.html

[U35] Py：发送邮件
来源：http://hz.yongpay.top/gtcfenfmbq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shuidangran.top/gtpemetlpf.html

[U36] Py：定时任务
来源：http://hz.cashguo.top/gtmemkszrd.html

schedule.every(10).minutes.do(job)
来源：http://hz.yuxming.cn/gtwrlbuidc.html

[U37] Py：读写 Excel
来源：http://hz.havefunace.top/gtfugdfdam.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.chenlongwang.top/gthbzqltxm.html

[U38] Py：获取脚本所在目录
来源：http://hz.52xcode.cn/gtsdtudiue.html

Path(__file__).resolve().parent
来源：http://hz.cdnleiting.top/gtjvuahmim.html

[U39] Py：判断是否在交互环境
来源：http://hz.snrcjt.cn/gtjcfqbslu.html

sys.stdout.isatty()
来源：http://hz.zhixingplan.top/gtvlwvalpz.html

[U40] Py：打印到标准错误
来源：http://hz.xziqi.cn/gtznynzjks.html

print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gtgccmvfpe.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.dianchejie.cn/gtmccrbqml.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hywenlv.cn/gtrjzcodmy.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xuetiantiany.cn/gtmimqtetx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.andypj.xyz/gtggwdcuqd.html

[U43] PHP：声明命名空间
来源：http://hz.sysykeji.top/gtltscconk.html

namespace App\Http;
来源：http://hz.tanke756.top/gtmkybsnlm.html

[U44] PHP：开启严格类型
来源：http://hz.pycfn.com/gtbxluysuh.html

declare(strict_types=1);
来源：http://hz.jyoumei.cn/gtociknqkw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gzhubu.top/gtqhswvkzz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtvaybktzh.html

[U46] PHP：可空类型
来源：http://hz.c1oappe.top/gtznrrccay.html

?string $name = null
来源：http://hz.ydzc1.top/gtcatfvyjy.html

[U47] PHP：联合类型
来源：http://hz.hfpthk.cn/gtqicmmqrn.html

int|string $id
来源：http://hz.ydjk.org.cn/gtmzcooseo.html

[U48] PHP：纯枚举
来源：http://hz.sxryk.cn/gthikufsdq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cdnleiting.top/gttcouaulv.html

[U49] PHP：只读属性
来源：http://hz.nanxuanxn.top/gtjfypdvul.html

public readonly string $name
来源：http://hz.gaohongyu789.top/gtwfpcfgog.html

[U50] PHP：构造器属性提升
来源：http://hz.jiagoushi.top/gthijiujzf.html

public function __construct(private int $id) {}
来源：http://hz.tanke756.top/gtxvxongnb.html

[U51] PHP：数组解构
来源：http://hz.c1oappe.top/gtwyduuoba.html

[$a, $b] = $arr;
来源：http://hz.yonumen.top/gtzyuyugxs.html

[U52] PHP：箭头函数
来源：http://hz.zhongyouzk.top/gtfgjavdgt.html

$double = fn($x) => $x * 2;
来源：http://hz.vqdsnc.cn/gtwydfbayg.html

[U53] PHP：空合并运算符
来源：http://hz.tianlin.xyz/gtqgbfgfph.html

$v = $a ?? $b ?? "default";
来源：http://hz.svipenyu.cn/gtbylwnojj.html

[U54] PHP：空安全调用
来源：http://hz.shanyushiyangtech.top/gtskspskie.html

$obj?->method()
来源：http://hz.daxiang520.top/gtpjrdpdvn.html

[U55] PHP：match 表达式
来源：http://hz.cqqwz.cn/gtwfqotzhd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258888.top/gtixuqkhje.html

[U56] PHP：命名参数
来源：http://hz.hammf.cn/gtxcsnsxzj.html

f(a: 1, b: 2)
来源：http://hz.sweek.top/gtibrkfhsz.html

[U57] PHP：字符串插值
来源：http://hz.yonumen.top/gtqmlopezq.html

"值: {$a}"
来源：http://hz.zhoulong.xyz/gtuskhtphn.html

[U58] PHP：数组三件套
来源：http://hz.dianchejie.cn/gtcgvubtoy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.andypj.xyz/gtmwkdrvss.html

[U59] PHP：自定义排序
来源：http://hz.xuetiantiany.cn/gtxglorcmr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtwxlxxjqb.html

[U60] PHP：JSON 编解码
来源：http://hz.vqdsnc.cn/gtokyreafc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jlsjyb.cn/gtvcemcmbz.html

[U61] PHP：正则
来源：http://hz.cashguo.top/gtnjkgwptb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtespjwrhd.html

[U62] PHP：日期对象
来源：http://hz.c1oappe.top/gtiqxzmpag.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gaohongyu789.top/gtnenmises.html

[U63] PHP：文件读写
来源：http://hz.iojbl.cn/gtxbsmvfpg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.feifeiyinyue.top/gthasgmkbw.html

[U64] PHP：目录遍历
来源：http://hz.feifeiyinyue.top/gtkcjsqlpi.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jinghuilouyu.cn/gtwxnetafu.html

[U65] PHP：会话
来源：http://hz.svipenyu.cn/gtlzdninfp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hnqzz.top/gtiusvxqon.html

[U66] PHP：设置 Cookie
来源：http://hz.chenlongwang.top/gtmgrakugf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinqigfzy.top/gtziwkjmlg.html

[U67] PHP：处理文件上传
来源：http://hz.snrcjt.cn/gtowkrajqn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.mhx1999.top/gtcmqlojax.html

[U68] PHP：PDO 连接
来源：http://hz.tian-w.cn/gtiphoovxs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hfpthk.cn/gtoorpkgxm.html

[U69] PHP：PDO 预处理
来源：http://hz.316326.xyz/gtfhrmoyql.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhixingplan.top/gtssbtuqqs.html

[U70] PHP：PDO 事务
来源：http://hz.yvedp.cn/gtgfohzmru.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jyoumei.cn/gtavfogvww.html

[U71] PHP：抛出异常
来源：http://hz.nanxinkj.top/gtogyifhby.html

throw new RuntimeException("失败", 500);
来源：http://hz.gzhubu.top/gthzbnyctp.html

[U72] PHP：写错误日志
来源：http://hz.andypj.xyz/gtrlrmwkmd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cucudq.cn/gtdvtnlibr.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydjk.org.cn/gtvgzleglu.html

parse_ini_file("config.ini", true)
来源：http://hz.shanyushiyangtech.top/gtztoykipj.html

[U74] PHP：读取环境变量
来源：http://hz.yonumen.top/gtlodacgfp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhijiandao.cn/gtavpevxdm.html

[U75] PHP：依赖注入
来源：http://hz.nanxuanxn.top/gtxrrbxftz.html

composer require psr/container
来源：http://hz.jinyuanbaomall.cn/gtefgmjqnd.html

[U76] PHP：简单路由
来源：http://hz.quarkkingdee.top/gtggrwyccd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shanyushiyangtech.top/gtvygwvedc.html

[U77] PHP：模板渲染
来源：http://hz.yongpay.top/gtvmzvzfsp.html

composer require twig/twig
来源：http://hz.fzhhl.top/gtjypnmtgm.html

[U78] PHP：单元测试
来源：http://hz.aibaodan.cn/gtvcgcgqwp.html

composer require --dev phpunit/phpunit
来源：http://hz.ehwqpu.com/gtsodvpyrx.html

[U79] PHP：静态分析
来源：http://hz.zhiwuduotai.top/gtqogyspfr.html

composer require --dev phpstan/phpstan
来源：http://hz.jinghuilouyu.cn/gtutmzlcot.html

[U80] PHP：代码规范修复
来源：http://hz.vqdsnc.cn/gtrqfovbhh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.9152youxi.cn/gtkqzgmyrf.html

[U81] JS：初始化项目
来源：http://hz.smart0.xyz/gtestppmjk.html

npm init -y;  npm i express
来源：http://hz.kuanghao11.cn/gtryeonrlu.html

[U82] JS：package.json 脚本
来源：http://hz.shzxlz.cn/gtvgehawyy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yangfankeji.com/gtexvajwbk.html

[U83] JS：ES Module 导入导出
来源：http://hz.chenzaomai.com/gtgotonsrl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenlongwang.top/gtpkbshoyo.html

[U84] JS：CommonJS 写法
来源：http://hz.cucudq.cn/gtzfuarryy.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yj20258888.top/gtsgvotqwo.html

[U85] JS：可选链
来源：http://hz.hysaishi.cn/gtrjparyww.html

a?.b?.c
来源：http://hz.ybcxt.top/gtxlzaoswo.html

[U86] JS：空值合并
来源：http://hz.yonumen.top/gtoxcewbsh.html

a ?? b
来源：http://hz.xziqi.cn/gttrppkwry.html

[U87] JS：解构默认值
来源：http://hz.gotoacloud.top/gtfwkwwxhr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.c1oappe.top/gtauqojusd.html

[U88] JS：对象展开合并
来源：http://hz.yj202588.top/gtsahlvpax.html

{ ...a, ...b }
来源：http://hz.yj202588.top/gtozryfzkd.html

[U89] JS：数组去重
来源：http://hz.yuxming.cn/gtmpncnuov.html

[...new Set(arr)]
来源：http://hz.cdnleiting.top/gtkbdykjwp.html

[U90] JS：数字数组排序
来源：http://hz.guowangkeji.top/gtbkrdtmra.html

[...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtnrdnivob.html

[U91] JS：对象键值遍历
来源：http://hz.jiagoushi.top/gtpynapbai.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zdqjudy.top/gtuofrtrrv.html

[U92] JS：深拷贝
来源：http://hz.9152youxi.cn/gtzwmjtnkv.html

structuredClone(obj)
来源：http://hz.haohaochexian.top/gtsvdkfeqv.html

[U93] JS：模板字符串
来源：http://hz.tanke756.top/gteoqluwcl.html

`共 ${n} 条`
来源：http://hz.shuidangran.top/gtcduulddd.html

[U94] JS：箭头函数
来源：http://hz.birdmap.top/gtilqhezxt.html

const double = x => x * 2;
来源：http://hz.zhiwuduotai.top/gtjqxxgjse.html

[U95] JS：Promise 包装
来源：http://hz.yonumen.top/gttycbaiqv.html

new Promise((resolve, reject) => {})
来源：http://hz.jyoumei.cn/gtkflrxxti.html

[U96] JS：async/await 与异常
来源：http://hz.ydjk.org.cn/gttcndtrow.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtlahbzodt.html

[U97] JS：并发请求
来源：http://hz.xuanzx.com/gtgswsjmny.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtocwqhdel.html

[U98] JS：fetch 带 JSON
来源：http://hz.fzhhl.top/gtdfbwuxci.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhengqikj.top/gtujowliso.html

[U99] JS：事件监听
来源：http://hz.hnqzz.top/gtambuujyk.html

el.addEventListener("click", e => {})
来源：http://hz.aibaodan.cn/gtjbcqrnpi.html

[U100] JS：DOM 查询
来源：http://hz.svipenyu.cn/gtnsnkkiyu.html

document.querySelector(".item")
来源：http://hz.hfpthk.cn/gtturpjtoc.html

[U101] JS：classList 操作
来源：http://hz.dianchejie.cn/gtdvdrkhih.html

el.classList.toggle("active")
来源：http://hz.zhengqikj.top/gtnvmxvcfv.html

[U102] JS：本地存储
来源：http://hz.yonumen.top/gtitkqzhwr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.iojbl.cn/gtsegwzwgs.html

[U103] JS：定时器
来源：http://hz.feifeiyinyue.top/gtzwraixkn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sweek.top/gtgklvdohr.html

[U104] JS：防抖
来源：http://hz.tianlin.xyz/gtqmwamnxk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gticnguttz.html

[U105] JS：节流
来源：http://hz.sufxvd.cn/gtdnybumwf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.smart0.xyz/gtutvmejta.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gtzsmawmyf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hywenlv.cn/gtuhxalnks.html

[U107] JS：数字千分位
来源：http://hz.52xcode.cn/gtznguhlrf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ivvv.top/gtlgvhgrsr.html

[U108] JS：随机整数
来源：http://hz.aizwys.cn/gtfnofeais.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhiwuduotai.top/gtmhvhilqu.html

[U109] JS：数组分组
来源：http://hz.chenzaomai.com/gtjekzqwri.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhongyouzk.top/gtezijhbzz.html

[U110] JS：数组分块
来源：http://hz.316326.xyz/gtnsldqupg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ehwqpu.com/gtuvzrhmep.html

[U111] JS：对象转 Map
来源：http://hz.dianchejie.cn/gtwibhdykr.html

new Map(Object.entries(obj))
来源：http://hz.svipenyu.cn/gtthiawbrd.html

[U112] JS：字符串补位
来源：http://hz.tianlin.xyz/gtanywedxe.html

"7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtdayvizop.html

[U113] JS：正则替换全部
来源：http://hz.snrcjt.cn/gtfgrxqqyg.html

s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtzonxolyh.html

[U114] JS：JSON 深比较
来源：http://hz.cdnleiting.top/gtlxqgouol.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gtywughdtb.html

[U115] JS：生成 UUID
来源：http://hz.xinyue.icu/gtmvryohft.html

crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtsbnqealp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tian-w.cn/gtibgcjrbc.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hnxiangtu.top/gtxngmfjau.html

[U117] JS：单元测试
来源：http://hz.jqgufenzy.top/gtwfprsmrm.html

npm i -D vitest;  npx vitest
来源：http://hz.quarkkingdee.top/gtvyakqhbg.html

[U118] JS：开发服务器
来源：http://hz.yuxming.cn/gtiyqowxgk.html

npm i -D vite;  npx vite
来源：http://hz.zhengqikj.top/gtppirkvxk.html

[U119] JS：生产构建
来源：http://hz.andypj.xyz/gtptdwcswl.html

npx vite build
来源：http://hz.jlsjyb.cn/gtffarbbug.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xziqi.cn/gtzprhgucr.html

import.meta.env.VITE_API_URL
来源：http://hz.zhoulong.xyz/gtggwnxvem.html

================================================================================
来源：http://hz.ppjwa.cn/gtvxvpbmtg.html

统计汇总
来源：http://hz.xziqi.cn/gtxxogsntf.html

================================================================================
来源：http://hz.ybcxt.top/gteqxckpkp.html

按语言统计（条）：
来源：http://hz.jinqigufen.top/gtcdboejjb.html

Python ......... 252
来源：http://hz.xingfuxueyuan.xyz/gtupnfbyib.html

PHP ............ 252
来源：http://hz.fzhhl.top/gtxcemevti.html

JavaScript ..... 252
来源：http://hz.cqqwz.cn/gthjlwugva.html

TypeScript ..... 212
来源：http://hz.xinyue.icu/gtimtlzsxo.html

Java ........... 212
来源：http://hz.fzhhl.top/gtujtcswnm.html

Go ............. 212
来源：http://hz.yuxming.cn/gtlofbpwim.html

Ruby ........... 212
来源：http://hz.kuanghao11.cn/gtcrdwejmf.html

C# ............. 212
来源：http://hz.gotoacloud.top/gtspuoqsfb.html

C .............. 30
来源：http://hz.yj202588.top/gtftzbqpfn.html

C++ ............ 30
来源：http://hz.jqgfzy.top/gtbtgyqqng.html

SQL ............ 90
来源：http://hz.cdnleiting.top/gtqxbgonie.html

Bash ........... 80
来源：http://hz.tian-w.cn/gtypwqgkkc.html

Kotlin ......... 15
来源：http://hz.ydjk.org.cn/gtlheehpml.html

Swift .......... 15
来源：http://hz.xuanzx.com/gtljxatsfw.html

Lua ............ 10
来源：http://hz.hywenlv.cn/gtlplkqzrn.html

Perl ........... 10
来源：http://hz.wangshuangyany.cn/gtxposchjj.html

Scala .......... 10
来源：http://hz.yuanzhike.top/gtfticsqnb.html

------------------------------------
来源：http://hz.hfpthk.cn/gtsnajfsue.html

合计 ........... 2106 条
来源：http://hz.xinyue.icu/gtgftlikhn.html

按章节统计：
来源：http://hz.jiagoushi.top/gtgxolgnmq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jqgfzy.top/gtgjqcwmbf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gtvjqcbong.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtjvqsapkp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gtkaidgaqt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhongyouzk.top/gtoiujhybs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtbcdkljkf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gzhubu.top/gtghkafcxm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.smart0.xyz/gtstaqjgkk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ydjk.org.cn/gtbnfgipeu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yonumen.top/gtiasekmsl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtteamaxjh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtsvgzmxzu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtjuvzrgbz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jlsjyb.cn/gtrzyqejpz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shzxlz.cn/gtlkxwzuyq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtakmdndzw.html

Q SQL 专题                              90
来源：http://hz.jqgfzy.top/gtlfzfrmib.html

R Bash 专题                             80
来源：http://hz.yonumen.top/gtlkiqbvpv.html

S C / C++ 专题                          60
来源：http://hz.daria6918.cn/gtjvijfnpv.html

T 其他语言补充                          60
来源：http://hz.yuxming.cn/gtcgnhinel.html

U 高频实用片段                         120
来源：http://hz.hfpthk.cn/gtmgbowdla.html

------------------------------------
来源：http://hz.gogol.net.cn/gtstmaeebl.html

合计                                  2106 条
来源：http://hz.jinqigufen.top/gtckzdddzn.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtoibqlaps.html

使用提醒
来源：http://hz.quarkkingdee.top/gtuucrqicz.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtbztejyea.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.chenzaomai.com/gtkjvoyrwj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.tanke756.top/gtfksxenku.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ydzc1.top/gtuhfgnkto.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yuanzhike.top/gtjhohhebk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.daxiang520.top/gtgmmteksx.html

—— 文件结束 ——
来源：http://hz.cucudq.cn/gtjgodobda.html

================================================================================
来源：http://hz.fengsongda.top/gtyjddnzsc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ehwqpu.com/gtbfwwjapy.html

Common Programming Examples Cheat Book
来源：http://hz.jlsjyb.cn/gtoyvlyvpc.html

================================================================================
来源：http://hz.yangfankeji.com/gtxqsruzwl.html

【收录内容】
来源：http://hz.hongshengwenyu.top/gtorehyquq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinghuilouyu.cn/gtndtqrirt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xinyue.icu/gtgwawllvy.html

SQL · Bash · C · C++
来源：http://hz.9152youxi.cn/gtmxvtxuzx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xingfuxueyuan.xyz/gtlxbgmghm.html

【使用说明】
来源：http://hz.tian-w.cn/gtyzysdhrj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gzhubu.top/gtpftzgvno.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj20258888.top/gtfbyybhgf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shzxlz.cn/gtqikuaxhc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jqgfzy.top/gtaubkqegn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hongshengwenyu.top/gtxbtftxdf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yongpay.top/gtxrgfhcku.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ivvv.top/gtykeqikco.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.wangdashe.top/gtomrlawuu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jiagoushi.top/gtiymtonij.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.fzhhl.top/gtmcefbtyl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.pengpengdd.cyou/gthcthgvjw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yongpay.top/gtywhprrjo.html

【文件统计】
来源：http://hz.jinqigufen.top/gtepctkauh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.bjfxy.top/gtpqqdsdwj.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtuunlueid.html

目  录
来源：http://hz.daria6918.cn/gtchebjblz.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtybifqsgd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shangyingyoupin.top/gtilgpztwa.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj20258888.top/gtupekzfll.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtxvxmwecm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhengqikj.top/gtuvceoxvg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhongyouzk.top/gtohlgtiav.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jqgfzy.top/gtpcxickii.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhengqikj.top/gtpcljyptj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.316326.xyz/gtriisrnok.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtsmmtfzzc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jinghuilouyu.cn/gtmgskzvwf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtsihrpnnk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtfhgljrwx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gttgwkhawi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.0kj1m.cn/gttnrkzaqe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.chenzaomai.com/gtxjvuciar.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtqtdrhukt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.kuanghao11.cn/gtwdejbhog.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yuxming.cn/gtywxwvrhi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ywan-chungtsiang.top/gtojatvzea.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenlongwang.top/gtednxcpob.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.cdnleiting.top/gttkdtpvay.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgfrkbvkp.html

A. 基础语法与类型
来源：http://hz.pengpengdd.cyou/gthlcsjcdw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtksiunnuo.html

[A01] Hello World
来源：http://hz.guannengcc.top/gtkeorapoa.html

Py:   print("Hello, World!")
来源：http://hz.iojbl.cn/gtvcrcrxaf.html

PHP:  echo "Hello, World!";
来源：http://hz.gogol.net.cn/gtiooiemrg.html

JS:   console.log("Hello, World!");
来源：http://hz.hnxiangtu.top/gthghldwkp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.guannengcc.top/gtdzpxrglk.html

Java: System.out.println("Hello, World!");
来源：http://hz.sysykeji.top/gtszcsvqqm.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinqigfzy.top/gtmqecpwnq.html

Ruby: puts "Hello, World!"
来源：http://hz.sweek.top/gtpahynkjx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.52xcode.cn/gtcftweoih.html


<!-- 参考信息 -->