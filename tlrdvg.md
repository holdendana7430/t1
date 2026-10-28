代发 wailian999

[U23] Py：分块读取大文件
来源：http://hz.ivvv.top/gtrzbvjgvd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shangyingyoupin.top/gtsdqimjyt.html

[U24] Py：路径操作
来源：http://hz.sweek.top/gtaemlgkdh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj20258.top/gttkagjnew.html

[U25] Py：CSV 按字典读
来源：http://hz.c1oappe.top/gtxrhkhhmv.html

csv.DictReader(f)
来源：http://hz.hysaishi.cn/gtwrqvlcmo.html

[U26] Py：并发下载
来源：http://hz.haohaochexian.top/gtdshxysbt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nwbrower.top/gtehfcuere.html

[U27] Py：异步 HTTP
来源：http://hz.chenjidiqi.icu/gtfdxjgpgf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydzc1.top/gtsluflmgo.html

[U28] Py：类型别名
来源：http://hz.sweek.top/gtewaxgjem.html

UserId = int
来源：http://hz.52xcode.cn/gtxdtpjmlf.html

[U29] Py：属性校验
来源：http://hz.hysaishi.cn/gtrvwyzxal.html

@property 与 @x.setter 配合
来源：http://hz.jianghu66.top/gtegzllkjv.html

[U30] Py：数据类
来源：http://hz.sxryk.cn/gtfdyqckqr.html

@dataclass(slots=True)
来源：http://hz.ppjwa.cn/gtfqeqcwve.html

[U31] Py：单测
来源：http://hz.dianchejie.cn/gtqckskbwc.html

python -m pytest -q
来源：http://hz.shangyingyoupin.top/gtwpqqjvob.html

[U32] Py：代码格式化
来源：http://hz.nwbrower.top/gteuftkwbs.html

ruff format . && ruff check --fix .
来源：http://hz.ydjk.org.cn/gtiwohcwec.html

[U33] Py：打包发布
来源：http://hz.snrcjt.cn/gtcrggfpuv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xuetiantiany.cn/gtyzaloqxw.html

[U34] Py：判断编码
来源：http://hz.dianchejie.cn/gtmghxmfuz.html

chardet.detect(raw)
来源：http://hz.yanxiufei.cn/gtuwjrlbpu.html

[U35] Py：发送邮件
来源：http://hz.chenzaomai.com/gtgeoamvmi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhixingplan.top/gtyprlpole.html

[U36] Py：定时任务
来源：http://hz.zhiwuduotai.top/gtxxwvjxrp.html

schedule.every(10).minutes.do(job)
来源：http://hz.shangyingyoupin.top/gterdqzjip.html

[U37] Py：读写 Excel
来源：http://hz.zhaomingkeji.xyz/gtsvvskniu.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dianchejie.cn/gtedqkpcbi.html

[U38] Py：获取脚本所在目录
来源：http://hz.jinghuilouyu.cn/gtwypdhcwp.html

Path(__file__).resolve().parent
来源：http://hz.jianghu66.top/gtmetzriwr.html

[U39] Py：判断是否在交互环境
来源：http://hz.xingfuxueyuan.xyz/gtyxqbmsbe.html

sys.stdout.isatty()
来源：http://hz.shuidangran.top/gtqgqwecoe.html

[U40] Py：打印到标准错误
来源：http://hz.cashguo.top/gtljwhnswf.html

print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtydroygaz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.aizwys.cn/gtconbxzyn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.vqdsnc.cn/gtocgrmcre.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhiwuduotai.top/gtebonmaul.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ppjwa.cn/gtrdrxljxl.html

[U43] PHP：声明命名空间
来源：http://hz.xingfuxueyuan.xyz/gtckiytoup.html

namespace App\Http;
来源：http://hz.hongshengwenyu.top/gtoijnuaeg.html

[U44] PHP：开启严格类型
来源：http://hz.zhengqikj.top/gtmminlgxk.html

declare(strict_types=1);
来源：http://hz.nanxinkj.top/gtfwvideck.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hammf.cn/gtfptgxfjt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gthasvuumr.html

[U46] PHP：可空类型
来源：http://hz.chenlongwang.top/gtkiqabish.html

?string $name = null
来源：http://hz.zhengqikj.top/gtlcfzzmwk.html

[U47] PHP：联合类型
来源：http://hz.jinyuanbaomall.cn/gtyunmvmns.html

int|string $id
来源：http://hz.sufxvd.cn/gtcewotkgq.html

[U48] PHP：纯枚举
来源：http://hz.quarkkingdee.top/gtlqsfyute.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shzxlz.cn/gtmzljblgb.html

[U49] PHP：只读属性
来源：http://hz.yj20258.top/gtasaqxkpt.html

public readonly string $name
来源：http://hz.sweek.top/gtqxeccvqm.html

[U50] PHP：构造器属性提升
来源：http://hz.kuanghao11.cn/gtusbgoxvn.html

public function __construct(private int $id) {}
来源：http://hz.yvedp.cn/gtmvvpdgoa.html

[U51] PHP：数组解构
来源：http://hz.aibaodan.cn/gtheoxptkr.html

[$a, $b] = $arr;
来源：http://hz.bjfxy.top/gtlugzeyau.html

[U52] PHP：箭头函数
来源：http://hz.yanxiufei.cn/gtxudupexf.html

$double = fn($x) => $x * 2;
来源：http://hz.nwbrower.top/gtvcaumbxo.html

[U53] PHP：空合并运算符
来源：http://hz.aizwys.cn/gtjviyjokp.html

$v = $a ?? $b ?? "default";
来源：http://hz.yvedp.cn/gtrmyomowy.html

[U54] PHP：空安全调用
来源：http://hz.zhiwuduotai.top/gtxujjwceh.html

$obj?->method()
来源：http://hz.jlsjyb.cn/gtoddldcdv.html

[U55] PHP：match 表达式
来源：http://hz.jinqigfzy.top/gtkzvjolrk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.nanxinkj.top/gtximncekp.html

[U56] PHP：命名参数
来源：http://hz.quarkkingdee.top/gtwcucaglq.html

f(a: 1, b: 2)
来源：http://hz.dianchejie.cn/gtqjljzcdq.html

[U57] PHP：字符串插值
来源：http://hz.guowangkeji.top/gtejmostyv.html

"值: {$a}"
来源：http://hz.quarkkingdee.top/gtzzlgqzvw.html

[U58] PHP：数组三件套
来源：http://hz.chenjidiqi.icu/gtiqfbtzno.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.quarkkingdee.top/gtgvmbbrdd.html

[U59] PHP：自定义排序
来源：http://hz.yj20258888.top/gtajstfzld.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxinkj.top/gtvfntlczg.html

[U60] PHP：JSON 编解码
来源：http://hz.jianghu66.top/gttouioxzq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ywan-chungtsiang.top/gterwkztry.html

[U61] PHP：正则
来源：http://hz.chenzaomai.com/gtgnhuimxm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shzxlz.cn/gtgqecqlgx.html

[U62] PHP：日期对象
来源：http://hz.havefunace.top/gtwjhymrkb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinqigfzy.top/gtncuigiek.html

[U63] PHP：文件读写
来源：http://hz.yj202588.top/gtdfnpdgti.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhengqikj.top/gtyuglxupe.html

[U64] PHP：目录遍历
来源：http://hz.jinqigfzy.top/gtcwesmblf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.wangdashe.top/gtpghhhrsf.html

[U65] PHP：会话
来源：http://hz.jinyuanbaomall.cn/gtakqmygxz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhengqikj.top/gtnpnubaur.html

[U66] PHP：设置 Cookie
来源：http://hz.wangshuangyany.cn/gttozterhd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zycfv.cn/gtfeqsrkra.html

[U67] PHP：处理文件上传
来源：http://hz.zhongyouzk.top/gtdtllnozs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxinkj.top/gtcrxmcqlf.html

[U68] PHP：PDO 连接
来源：http://hz.yuanzhike.top/gthozyjngi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yueranfly.top/gtoaeszecn.html

[U69] PHP：PDO 预处理
来源：http://hz.sysykeji.top/gtoptxflyu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gogol.net.cn/gtwsehhorb.html

[U70] PHP：PDO 事务
来源：http://hz.fengsongda.top/gtrwmrqxgu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ybcxt.top/gtjgafwnef.html

[U71] PHP：抛出异常
来源：http://hz.jlsjyb.cn/gtcdnbzbyz.html

throw new RuntimeException("失败", 500);
来源：http://hz.nwbrower.top/gtixjwjyzr.html

[U72] PHP：写错误日志
来源：http://hz.wangdashe.top/gtrvqvqenk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hysaishi.cn/gtehohvaou.html

[U73] PHP：读取 ini 配置
来源：http://hz.shanyushiyangkeji.top/gtmgfxhkuq.html

parse_ini_file("config.ini", true)
来源：http://hz.yuanzhike.top/gttmkinxjf.html

[U74] PHP：读取环境变量
来源：http://hz.guannengcc.top/gtqtrgaiox.html

getenv("APP_ENV") ?: "production"
来源：http://hz.dashuyun.cn/gtxpksjrrn.html

[U75] PHP：依赖注入
来源：http://hz.redwolf501.top/gtsssxeojm.html

composer require psr/container
来源：http://hz.yuxming.cn/gtrhrcgzlg.html

[U76] PHP：简单路由
来源：http://hz.316326.xyz/gtkcodbxsh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.feifeiyinyue.top/gtvtutseif.html

[U77] PHP：模板渲染
来源：http://hz.cdnleiting.top/gtozycbyjq.html

composer require twig/twig
来源：http://hz.jiagoushi.top/gtrumkqrzo.html

[U78] PHP：单元测试
来源：http://hz.yuxming.cn/gtgvakqmjq.html

composer require --dev phpunit/phpunit
来源：http://hz.dianchejie.cn/gtteuslzqo.html

[U79] PHP：静态分析
来源：http://hz.iojbl.cn/gtvgrvrlkp.html

composer require --dev phpstan/phpstan
来源：http://hz.shuidangran.top/gthkjguoug.html

[U80] PHP：代码规范修复
来源：http://hz.xziqi.cn/gtgolozpos.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.daxiang520.top/gtjgeahkij.html

[U81] JS：初始化项目
来源：http://hz.ydzc1.top/gterouzncb.html

npm init -y;  npm i express
来源：http://hz.dianchejie.cn/gtdxmrfyig.html

[U82] JS：package.json 脚本
来源：http://hz.52xcode.cn/gtdmmmquwb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.fengsongda.top/gtgtmkxtgf.html

[U83] JS：ES Module 导入导出
来源：http://hz.9152youxi.cn/gtrawlwxpp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zdqjudy.top/gtcijlaedf.html

[U84] JS：CommonJS 写法
来源：http://hz.ydjk.org.cn/gtngacswde.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yanxiufei.cn/gtcwvkpfpr.html

[U85] JS：可选链
来源：http://hz.ehwqpu.com/gtiovfevae.html

a?.b?.c
来源：http://hz.aibaodan.cn/gthnpfoqch.html

[U86] JS：空值合并
来源：http://hz.snrcjt.cn/gtmpiwzrbg.html

a ?? b
来源：http://hz.dashuyun.cn/gtkqegvmme.html

[U87] JS：解构默认值
来源：http://hz.meibo888.top/gtlwaunfjn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhaomingkeji.xyz/gtojtoyzhr.html

[U88] JS：对象展开合并
来源：http://hz.cheryme.top/gtimrafabx.html

{ ...a, ...b }
来源：http://hz.sxryk.cn/gttbwvupyf.html

[U89] JS：数组去重
来源：http://hz.aibaodan.cn/gtendaykau.html

[...new Set(arr)]
来源：http://hz.birdmap.top/gtvmdxejmo.html

[U90] JS：数字数组排序
来源：http://hz.chenzaomai.com/gtdkllvjgk.html

[...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtveruqrmv.html

[U91] JS：对象键值遍历
来源：http://hz.xuetiantiany.cn/gtfuvbghto.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yonumen.top/gtjzkqaudm.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangtech.top/gtavkykakb.html

structuredClone(obj)
来源：http://hz.tianlin.xyz/gtjzezqcnh.html

[U93] JS：模板字符串
来源：http://hz.nwbrower.top/gtvldofwwy.html

`共 ${n} 条`
来源：http://hz.hfpthk.cn/gthegjmzer.html

[U94] JS：箭头函数
来源：http://hz.redwolf501.top/gtssgfkojd.html

const double = x => x * 2;
来源：http://hz.yueranfly.top/gtztlfbwjz.html

[U95] JS：Promise 包装
来源：http://hz.meibo888.top/gtypnitpvf.html

new Promise((resolve, reject) => {})
来源：http://hz.shanyushiyangkeji.top/gtvaydgtlp.html

[U96] JS：async/await 与异常
来源：http://hz.yvedp.cn/gtnbbmrtlu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtckmhrrlu.html

[U97] JS：并发请求
来源：http://hz.sxryk.cn/gtlsyexczu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtxhyusrry.html

[U98] JS：fetch 带 JSON
来源：http://hz.nanxinkj.top/gtxjrpugwc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hnqzz.top/gtkdnimlun.html

[U99] JS：事件监听
来源：http://hz.smart0.xyz/gtxgdopstp.html

el.addEventListener("click", e => {})
来源：http://hz.wangdashe.top/gtvgbkbqkg.html

[U100] JS：DOM 查询
来源：http://hz.hammf.cn/gtivxbqszw.html

document.querySelector(".item")
来源：http://hz.xziqi.cn/gtzuyfzbke.html

[U101] JS：classList 操作
来源：http://hz.pycfn.com/gtfwsvavbf.html

el.classList.toggle("active")
来源：http://hz.sweek.top/gtmgdzgkkl.html

[U102] JS：本地存储
来源：http://hz.cucudq.cn/gtjggjnwov.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zdqjudy.top/gtrokfpnen.html

[U103] JS：定时器
来源：http://hz.ydzc1.top/gtxwrqzpzm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.316326.xyz/gteiqqiwur.html

[U104] JS：防抖
来源：http://hz.zhixingplan.top/gtcyeruuga.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtsndovpgc.html

[U105] JS：节流
来源：http://hz.jiagoushi.top/gtocyszyar.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.vqdsnc.cn/gtcpiemssb.html

[U106] JS：日期格式化
来源：http://hz.yongpay.top/gttnmzmkos.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.pycfn.com/gtseaxuhjh.html

[U107] JS：数字千分位
来源：http://hz.shzxlz.cn/gtxyudyqps.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gotoacloud.top/gttzxfilqt.html

[U108] JS：随机整数
来源：http://hz.nwbrower.top/gttpbsbvvt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangkeji.top/gtrkupeecw.html

[U109] JS：数组分组
来源：http://hz.cucudq.cn/gtoknhpbnf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gtrslrfzuz.html

[U110] JS：数组分块
来源：http://hz.dianchejie.cn/gtydzivyzs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.aibaodan.cn/gthutjwqkw.html

[U111] JS：对象转 Map
来源：http://hz.yongpay.top/gtdmeaegud.html

new Map(Object.entries(obj))
来源：http://hz.ydzc1.top/gtbkjqiayz.html

[U112] JS：字符串补位
来源：http://hz.yuxming.cn/gtsibaoddm.html

"7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtoonlrpca.html

[U113] JS：正则替换全部
来源：http://hz.nanxuanxn.top/gttdiotuzv.html

s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gthwjiwsap.html

[U114] JS：JSON 深比较
来源：http://hz.hammf.cn/gtaylyimxb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtbnzacyyv.html

[U115] JS：生成 UUID
来源：http://hz.ybcxt.top/gtwnlcxgyo.html

crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gteukcnmpv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj202588.top/gtsifiekqi.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dianchejie.cn/gtuwrmjjrs.html

[U117] JS：单元测试
来源：http://hz.gotoacloud.top/gtfbdeheoz.html

npm i -D vitest;  npx vitest
来源：http://hz.quarkkingdee.top/gtpxreyped.html

[U118] JS：开发服务器
来源：http://hz.ivvv.top/gtxgmpmhrg.html

npm i -D vite;  npx vite
来源：http://hz.smart0.xyz/gthajtfgho.html

[U119] JS：生产构建
来源：http://hz.shzxlz.cn/gtbjxttgky.html

npx vite build
来源：http://hz.jqgufenzy.top/gtvmyxstfc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.svipenyu.cn/gtpenkvlzo.html

import.meta.env.VITE_API_URL
来源：http://hz.nanxinkj.top/gtumsjoaqh.html

================================================================================
来源：http://hz.cdnleiting.top/gtekgvjrnd.html

统计汇总
来源：http://hz.jinqigfzy.top/gtnnvymgle.html

================================================================================
来源：http://hz.jiagoushi.top/gtcozycokv.html

按语言统计（条）：
来源：http://hz.tian-w.cn/gtenljkqzu.html

Python ......... 252
来源：http://hz.jiagoushi.top/gtwgvbyjos.html

PHP ............ 252
来源：http://hz.316326.xyz/gtjcbubgjy.html

JavaScript ..... 252
来源：http://hz.xziqi.cn/gtyhglqiir.html

TypeScript ..... 212
来源：http://hz.nanxuanxn.top/gtqbgbyyff.html

Java ........... 212
来源：http://hz.zhijiandao.cn/gtxgmmvpbr.html

Go ............. 212
来源：http://hz.gaohongyu789.top/gtkbafrjio.html

Ruby ........... 212
来源：http://hz.hnqzz.top/gtcnonntha.html

C# ............. 212
来源：http://hz.xuanzx.com/gtlxkoypth.html

C .............. 30
来源：http://hz.hnqzz.top/gtqgizatxu.html

C++ ............ 30
来源：http://hz.hongshengwenyu.top/gtqfkmnbgw.html

SQL ............ 90
来源：http://hz.aibaodan.cn/gtpkhbhvos.html

Bash ........... 80
来源：http://hz.smart0.xyz/gtaiqmgzgf.html

Kotlin ......... 15
来源：http://hz.cheryme.top/gtvkrsayjx.html

Swift .......... 15
来源：http://hz.hnqzz.top/gtcvtidmoi.html

Lua ............ 10
来源：http://hz.svipenyu.cn/gtxvgfkitg.html

Perl ........... 10
来源：http://hz.xinyue.icu/gthfqjggwe.html

Scala .......... 10
来源：http://hz.hnqzz.top/gtlmfbtbgi.html

------------------------------------
来源：http://hz.pycfn.com/gtcyawcyov.html

合计 ........... 2106 条
来源：http://hz.shangyingyoupin.top/gtzxbnhpga.html

按章节统计：
来源：http://hz.fzhhl.top/gtcbabbhkv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhaomingkeji.xyz/gtgowmpsln.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtwpwqjtxs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangshuangyany.cn/gtmefvkwlw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shanyushiyangkeji.top/gtxmwdyrqe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.gotoacloud.top/gtyjrnztst.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ppjwa.cn/gtmupiihns.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtyjqnkzgp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tianlin.xyz/gtnzrrksju.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtcsvtnecs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gogol.net.cn/gtxeubsorq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtoomiodfm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtflztykxo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtbxsnijlk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.vqdsnc.cn/gtgqwspdey.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ywan-chungtsiang.top/gtdrgnqfmz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtixxjljpj.html

Q SQL 专题                              90
来源：http://hz.xziqi.cn/gtbbcoylsi.html

R Bash 专题                             80
来源：http://hz.yuxming.cn/gthuslvpvw.html

S C / C++ 专题                          60
来源：http://hz.jqgfzy.top/gtoeqbxooy.html

T 其他语言补充                          60
来源：http://hz.chenlongwang.top/gtwkwwpfhy.html

U 高频实用片段                         120
来源：http://hz.aizwys.cn/gtuszbzoxy.html

------------------------------------
来源：http://hz.jqgufenzy.top/gtbliyfwrs.html

合计                                  2106 条
来源：http://hz.ivvv.top/gtrtspnhmi.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtyewhouss.html

使用提醒
来源：http://hz.shanyushiyangkeji.top/gtkpqpvidx.html

--------------------------------------------------------------------------------
来源：http://hz.zhengqikj.top/gtipblsere.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shanyushiyangkeji.top/gtcsvcyywm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.fengsongda.top/gthpulygmk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj20258.top/gtorkdyagk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yangfankeji.com/gtraoasyea.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shanyushiyangkeji.top/gtpitbqtqo.html

—— 文件结束 ——
来源：http://hz.havefunace.top/gtfionnnfb.html

================================================================================
来源：http://hz.yonumen.top/gttefeqmqb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.cqqwz.cn/gtagbnlmiw.html

Common Programming Examples Cheat Book
来源：http://hz.haohaochexian.top/gtcrmmrczp.html

================================================================================
来源：http://hz.snrcjt.cn/gtkacnzocb.html

【收录内容】
来源：http://hz.snrcjt.cn/gtdwtzyizw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.chenzaomai.com/gtyrelodlu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhijiandao.cn/gtsqekzzdq.html

SQL · Bash · C · C++
来源：http://hz.havefunace.top/gtklxindnv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydzc1.top/gtokfeooaw.html

【使用说明】
来源：http://hz.nanxinkj.top/gtiesjambv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cdnleiting.top/gtvzbsgevq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.kuanghao11.cn/gtjbohewyd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.c1oappe.top/gtvcumslej.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yanxiufei.cn/gtnxevpmze.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.316326.xyz/gtfsgxgtto.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ydzc1.top/gtyjiokxgu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ydjk.org.cn/gtncubikqm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.52xcode.cn/gtxpwytgor.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinghuilouyu.cn/gtznbngqli.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhijiandao.cn/gtqveywzyu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.havefunace.top/gtdworqspe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hnqzz.top/gtxlqdgrsd.html

【文件统计】
来源：http://hz.ppjwa.cn/gtbtbknkvi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ydjk.org.cn/gtlfwesjqa.html

--------------------------------------------------------------------------------
来源：http://hz.aizwys.cn/gtvsacysfi.html

目  录
来源：http://hz.wangdashe.top/gtplrwrkjz.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtgxgdnlll.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xuanzx.com/gthvdcrlhc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhongyouzk.top/gtvoyffbco.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jinghuilouyu.cn/gtlowyloez.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.tianlin.xyz/gtynhrmpaf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nanxuanxn.top/gtnytvvjsg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.9152youxi.cn/gtnzuhysqt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gogol.net.cn/gtcnjkxatp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.haohaochexian.top/gtgavahfxt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtzemcofoj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yongpay.top/gtdunjeonx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtfxmxnnwb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtxkogigyw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtdodjtjtf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jinghuilouyu.cn/gtrpzhhdbk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sysykeji.top/gthykosypd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtfjsyxpui.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.wangshuangyany.cn/gtnemlakfy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jianghu66.top/gthagtnaop.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yj20258888.top/gtmbzgqpcu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gttlglhhcg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtfukhyyji.html


<!-- 参考信息 -->