代发 wailian999

[U23] Py：分块读取大文件
来源：http://hz.cucudq.cn/gtsypqmmra.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.0kj1m.cn/gttzglgxma.html

[U24] Py：路径操作
来源：http://hz.guannengcc.top/gtzowguckj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cdnleiting.top/gtdbkwmtho.html

[U25] Py：CSV 按字典读
来源：http://hz.cucudq.cn/gtcbmnaopt.html

csv.DictReader(f)
来源：http://hz.gotoacloud.top/gthrqberdi.html

[U26] Py：并发下载
来源：http://hz.52xcode.cn/gtbrrooegd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xylfe.cn/gtfzexcoys.html

[U27] Py：异步 HTTP
来源：http://hz.guowangkeji.top/gteqtbwbcz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.iojbl.cn/gtclqgvnxn.html

[U28] Py：类型别名
来源：http://hz.cdnleiting.top/gtowagwjmz.html

UserId = int
来源：http://hz.hnqzz.top/gtgczygeaf.html

[U29] Py：属性校验
来源：http://hz.xingfuxueyuan.xyz/gtlkdexbhb.html

@property 与 @x.setter 配合
来源：http://hz.redwolf501.top/gtwezanqnw.html

[U30] Py：数据类
来源：http://hz.shzxlz.cn/gthwjlnbti.html

@dataclass(slots=True)
来源：http://hz.hfpthk.cn/gtxdezirha.html

[U31] Py：单测
来源：http://hz.52xcode.cn/gtemvslamz.html

python -m pytest -q
来源：http://hz.cqqwz.cn/gtrpbmlbxm.html

[U32] Py：代码格式化
来源：http://hz.sufxvd.cn/gthcecjjog.html

ruff format . && ruff check --fix .
来源：http://hz.svipenyu.cn/gtlxyaimok.html

[U33] Py：打包发布
来源：http://hz.xylfe.cn/gtccbtyumf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xziqi.cn/gtqagwykeb.html

[U34] Py：判断编码
来源：http://hz.cqqwz.cn/gtaurkoyap.html

chardet.detect(raw)
来源：http://hz.yueranfly.top/gtbvzbvtac.html

[U35] Py：发送邮件
来源：http://hz.sysykeji.top/gtckdxfldj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.52xcode.cn/gthdbrljxj.html

[U36] Py：定时任务
来源：http://hz.ybcxt.top/gtzrfgkqvz.html

schedule.every(10).minutes.do(job)
来源：http://hz.mhx1999.top/gtublzfsfy.html

[U37] Py：读写 Excel
来源：http://hz.sysykeji.top/gtzdwbnwme.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hongshengwenyu.top/gtpgdnhuqz.html

[U38] Py：获取脚本所在目录
来源：http://hz.jyoumei.cn/gtbfmtknwo.html

Path(__file__).resolve().parent
来源：http://hz.chenlongwang.top/gtkyxutimw.html

[U39] Py：判断是否在交互环境
来源：http://hz.316326.xyz/gtbebdlanq.html

sys.stdout.isatty()
来源：http://hz.ehwqpu.com/gtthvluezx.html

[U40] Py：打印到标准错误
来源：http://hz.hfpthk.cn/gtomldcdje.html

print("err", file=sys.stderr)
来源：http://hz.hongshengwenyu.top/gtknubkjef.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.pycfn.com/gtcwavgiqf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.havefunace.top/gtjlcaishy.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yj20258.top/gtorcxcczr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.tian-w.cn/gtgkmfrzty.html

[U43] PHP：声明命名空间
来源：http://hz.yuxming.cn/gtvkipuucj.html

namespace App\Http;
来源：http://hz.dianchejie.cn/gtahqgexlr.html

[U44] PHP：开启严格类型
来源：http://hz.snrcjt.cn/gtqycjqoke.html

declare(strict_types=1);
来源：http://hz.yj20258.top/gtjrevobbb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.dianchejie.cn/gtmgmlbzxc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtphcflgqn.html

[U46] PHP：可空类型
来源：http://hz.sysykeji.top/gtvflqrvzw.html

?string $name = null
来源：http://hz.ybcxt.top/gtrlqczsuy.html

[U47] PHP：联合类型
来源：http://hz.ppjwa.cn/gtjehjfwdc.html

int|string $id
来源：http://hz.jinqigfzy.top/gtwwblqqzg.html

[U48] PHP：纯枚举
来源：http://hz.guowangkeji.top/gtcwfkgqbe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ehwqpu.com/gtxoxmgtsg.html

[U49] PHP：只读属性
来源：http://hz.nanxuanxn.top/gtdvuzqbps.html

public readonly string $name
来源：http://hz.meibo888.top/gtyiypkypr.html

[U50] PHP：构造器属性提升
来源：http://hz.yonumen.top/gtbleflsaj.html

public function __construct(private int $id) {}
来源：http://hz.fzhhl.top/gttrknaetx.html

[U51] PHP：数组解构
来源：http://hz.chenlongwang.top/gtcwfjqioa.html

[$a, $b] = $arr;
来源：http://hz.ppjwa.cn/gtsziodxuw.html

[U52] PHP：箭头函数
来源：http://hz.vqdsnc.cn/gtndhpmdwe.html

$double = fn($x) => $x * 2;
来源：http://hz.daxiang520.top/gtsjrhvkrb.html

[U53] PHP：空合并运算符
来源：http://hz.yongpay.top/gtqyyqivnk.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnqzz.top/gtfhieuxsa.html

[U54] PHP：空安全调用
来源：http://hz.hnqzz.top/gtpsjpdhkr.html

$obj?->method()
来源：http://hz.ehwqpu.com/gtqytpvmpw.html

[U55] PHP：match 表达式
来源：http://hz.fengsongda.top/gtleysahvn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ydzc1.top/gtpgxgkquu.html

[U56] PHP：命名参数
来源：http://hz.zhengqikj.top/gtpxnmlgtz.html

f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtwxhxhood.html

[U57] PHP：字符串插值
来源：http://hz.sufxvd.cn/gtnislytmv.html

"值: {$a}"
来源：http://hz.nwbrower.top/gtuertqnmu.html

[U58] PHP：数组三件套
来源：http://hz.kuanghao11.cn/gtjvzqwcde.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sysykeji.top/gtndonmckt.html

[U59] PHP：自定义排序
来源：http://hz.316326.xyz/gtaucrobux.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.snrcjt.cn/gtwsojwivq.html

[U60] PHP：JSON 编解码
来源：http://hz.sweek.top/gtshrvtcjo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ybcxt.top/gtytnrugjy.html

[U61] PHP：正则
来源：http://hz.cqqwz.cn/gtzzdqiyid.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtyciwyquq.html

[U62] PHP：日期对象
来源：http://hz.redwolf501.top/gtrqnqxeaz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhiwuduotai.top/gtyzyfbmer.html

[U63] PHP：文件读写
来源：http://hz.daria6918.cn/gtboszrpvq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.redwolf501.top/gtsnerylzx.html

[U64] PHP：目录遍历
来源：http://hz.tanke756.top/gtttnhzxdr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhixingplan.top/gtojrbjeaf.html

[U65] PHP：会话
来源：http://hz.redwolf501.top/gtizuodxik.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yangfankeji.com/gtuhdydsjt.html

[U66] PHP：设置 Cookie
来源：http://hz.zhengqikj.top/gtqvvckgwd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sysykeji.top/gtranttpzm.html

[U67] PHP：处理文件上传
来源：http://hz.jinghuilouyu.cn/gtgyfwblth.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.c1oappe.top/gtngprbhzo.html

[U68] PHP：PDO 连接
来源：http://hz.jqgufenzy.top/gtvvtvcxkd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hysaishi.cn/gtaclujkwi.html

[U69] PHP：PDO 预处理
来源：http://hz.xuanzx.com/gtcpaofnax.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tianlin.xyz/gtpodgtlds.html

[U70] PHP：PDO 事务
来源：http://hz.dashuyun.cn/gtjpvwphur.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cdnleiting.top/gtppovonfk.html

[U71] PHP：抛出异常
来源：http://hz.hysaishi.cn/gtivftohbl.html

throw new RuntimeException("失败", 500);
来源：http://hz.guowangkeji.top/gtpwjktqdw.html

[U72] PHP：写错误日志
来源：http://hz.zhongyouzk.top/gtuchzivpr.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cheryme.top/gtmovsatyg.html

[U73] PHP：读取 ini 配置
来源：http://hz.sysykeji.top/gtctqhphtn.html

parse_ini_file("config.ini", true)
来源：http://hz.shuidangran.top/gtsrkwklwz.html

[U74] PHP：读取环境变量
来源：http://hz.jyoumei.cn/gtlnxueplx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.c1oappe.top/gtrqkbagva.html

[U75] PHP：依赖注入
来源：http://hz.chenzaomai.com/gtvvmqbmae.html

composer require psr/container
来源：http://hz.zhongyouzk.top/gtzmrfgywg.html

[U76] PHP：简单路由
来源：http://hz.0kj1m.cn/gtvbnpjkkc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.iojbl.cn/gtyhopwtbp.html

[U77] PHP：模板渲染
来源：http://hz.hysaishi.cn/gtsaxqpyue.html

composer require twig/twig
来源：http://hz.wangshuangyany.cn/gtntbszfvf.html

[U78] PHP：单元测试
来源：http://hz.zhengqikj.top/gtjpyugryv.html

composer require --dev phpunit/phpunit
来源：http://hz.9152youxi.cn/gttdhfvbqh.html

[U79] PHP：静态分析
来源：http://hz.aibaodan.cn/gttftnqmys.html

composer require --dev phpstan/phpstan
来源：http://hz.ybcxt.top/gtbfnugphp.html

[U80] PHP：代码规范修复
来源：http://hz.cdnleiting.top/gtpbvfccdd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cashguo.top/gtwuruaqff.html

[U81] JS：初始化项目
来源：http://hz.quarkkingdee.top/gtjcwktgzv.html

npm init -y;  npm i express
来源：http://hz.xingfuxueyuan.xyz/gtkjepsczz.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtetqpcpsl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shanyushiyangtech.top/gtjmlbxctm.html

[U83] JS：ES Module 导入导出
来源：http://hz.hysaishi.cn/gtljnmhkzy.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yuanzhike.top/gtjhhupqbo.html

[U84] JS：CommonJS 写法
来源：http://hz.zhaomingkeji.xyz/gtzkolhyfy.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jianghu66.top/gtdkwmcuek.html

[U85] JS：可选链
来源：http://hz.jinqigufen.top/gtmsaiggxn.html

a?.b?.c
来源：http://hz.cdnleiting.top/gtxoqwqzpb.html

[U86] JS：空值合并
来源：http://hz.52xcode.cn/gtgkargljt.html

a ?? b
来源：http://hz.zhaomingkeji.xyz/gtuhhwzgbp.html

[U87] JS：解构默认值
来源：http://hz.dashuyun.cn/gtmedyszlr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.mhx1999.top/gtpxneoavn.html

[U88] JS：对象展开合并
来源：http://hz.meibo888.top/gthwgyftok.html

{ ...a, ...b }
来源：http://hz.hfpthk.cn/gtkjyaiish.html

[U89] JS：数组去重
来源：http://hz.hammf.cn/gtfsdsdweh.html

[...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtojkrxvyj.html

[U90] JS：数字数组排序
来源：http://hz.iojbl.cn/gtxoeissnp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtcyfocqpq.html

[U91] JS：对象键值遍历
来源：http://hz.daxiang520.top/gtdkiawrdd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hnxiangtu.top/gtraevvkkd.html

[U92] JS：深拷贝
来源：http://hz.cdnleiting.top/gtcqoosver.html

structuredClone(obj)
来源：http://hz.snrcjt.cn/gtlziwjwpw.html

[U93] JS：模板字符串
来源：http://hz.jinyuanbaomall.cn/gtgfheapoz.html

`共 ${n} 条`
来源：http://hz.birdmap.top/gtbplksqjn.html

[U94] JS：箭头函数
来源：http://hz.xinyue.icu/gtimeulddh.html

const double = x => x * 2;
来源：http://hz.cqqwz.cn/gtsczuubku.html

[U95] JS：Promise 包装
来源：http://hz.hysaishi.cn/gtwlvcghtv.html

new Promise((resolve, reject) => {})
来源：http://hz.ehwqpu.com/gthrgmgxlp.html

[U96] JS：async/await 与异常
来源：http://hz.cqqwz.cn/gthamdlpvd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yuxming.cn/gtjnrerxsy.html

[U97] JS：并发请求
来源：http://hz.gotoacloud.top/gtcbutiogk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtoqfvrmgk.html

[U98] JS：fetch 带 JSON
来源：http://hz.vqdsnc.cn/gtxgfxenji.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hywenlv.cn/gtsxfqloat.html

[U99] JS：事件监听
来源：http://hz.hongshengwenyu.top/gtrfuiftba.html

el.addEventListener("click", e => {})
来源：http://hz.pengpengdd.cyou/gtikuujkha.html

[U100] JS：DOM 查询
来源：http://hz.dianchejie.cn/gthwgxpvpx.html

document.querySelector(".item")
来源：http://hz.tanke756.top/gtwggfdpbq.html

[U101] JS：classList 操作
来源：http://hz.havefunace.top/gtpmtmtkya.html

el.classList.toggle("active")
来源：http://hz.hnxiangtu.top/gtoesavzyw.html

[U102] JS：本地存储
来源：http://hz.gogol.net.cn/gtgrztrrjz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jianghu66.top/gtipspcdor.html

[U103] JS：定时器
来源：http://hz.zhoulong.xyz/gtvncohktm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.9152youxi.cn/gtjjrwmvtz.html

[U104] JS：防抖
来源：http://hz.ywan-chungtsiang.top/gtetzvwwkx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtdffdtgtg.html

[U105] JS：节流
来源：http://hz.jiagoushi.top/gtoyuocdpw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuanzhike.top/gtpbuxrcqk.html

[U106] JS：日期格式化
来源：http://hz.yvedp.cn/gtnqbzzpgx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxuanxn.top/gtmqzgsixa.html

[U107] JS：数字千分位
来源：http://hz.cdnleiting.top/gtlhlmeiwb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.bjfxy.top/gtlstljwos.html

[U108] JS：随机整数
来源：http://hz.fengsongda.top/gtesffdkeg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangkeji.top/gteoqpsqef.html

[U109] JS：数组分组
来源：http://hz.xuanzx.com/gtpwaohbfl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtuhdhcdrg.html

[U110] JS：数组分块
来源：http://hz.daxiang520.top/gtcfazyuyk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhiwuduotai.top/gtjxgrszed.html

[U111] JS：对象转 Map
来源：http://hz.shangyingyoupin.top/gtgtbxormr.html

new Map(Object.entries(obj))
来源：http://hz.xuetiantiany.cn/gtxvkkntcq.html

[U112] JS：字符串补位
来源：http://hz.guannengcc.top/gtikacnusg.html

"7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtfdqnidmg.html

[U113] JS：正则替换全部
来源：http://hz.ivvv.top/gtpwwdaspu.html

s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtvrsdiafy.html

[U114] JS：JSON 深比较
来源：http://hz.sweek.top/gtxnrtxrsb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtumehxbbw.html

[U115] JS：生成 UUID
来源：http://hz.gotoacloud.top/gtqqeeaevr.html

crypto.randomUUID()
来源：http://hz.cheryme.top/gtqmtbnide.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yueranfly.top/gtsulvfvey.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xingfuxueyuan.xyz/gtxuvrkoqn.html

[U117] JS：单元测试
来源：http://hz.cashguo.top/gtsbypmrkn.html

npm i -D vitest;  npx vitest
来源：http://hz.shanyushiyangkeji.top/gtogfuhlfu.html

[U118] JS：开发服务器
来源：http://hz.jinqigfzy.top/gtaxbpxvxv.html

npm i -D vite;  npx vite
来源：http://hz.mhx1999.top/gtrmhoasuk.html

[U119] JS：生产构建
来源：http://hz.yongpay.top/gtumonhyjp.html

npx vite build
来源：http://hz.xinyue.icu/gthjvaqbxx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.daria6918.cn/gtyxibvcmj.html

import.meta.env.VITE_API_URL
来源：http://hz.hongshengwenyu.top/gtwggwayhr.html

================================================================================
来源：http://hz.jiagoushi.top/gtnkcasidd.html

统计汇总
来源：http://hz.sufxvd.cn/gtghiogqbz.html

================================================================================
来源：http://hz.sxryk.cn/gtklzqhjjn.html

按语言统计（条）：
来源：http://hz.gaohongyu789.top/gtcpleslrw.html

Python ......... 252
来源：http://hz.xziqi.cn/gtdfgxbnce.html

PHP ............ 252
来源：http://hz.haohaochexian.top/gtevpiytsz.html

JavaScript ..... 252
来源：http://hz.daria6918.cn/gtoczpjash.html

TypeScript ..... 212
来源：http://hz.bjfxy.top/gtlayebhsb.html

Java ........... 212
来源：http://hz.hnqzz.top/gtyffujppr.html

Go ............. 212
来源：http://hz.nanxuanxn.top/gtoderkslf.html

Ruby ........... 212
来源：http://hz.jlsjyb.cn/gtydylvtxm.html

C# ............. 212
来源：http://hz.pengpengdd.cyou/gtxdubndnr.html

C .............. 30
来源：http://hz.andypj.xyz/gtdnxxmxtd.html

C++ ............ 30
来源：http://hz.birdmap.top/gtdnksruzs.html

SQL ............ 90
来源：http://hz.gzhubu.top/gtjvurzfru.html

Bash ........... 80
来源：http://hz.kuanghao11.cn/gtmplhgbtm.html

Kotlin ......... 15
来源：http://hz.mhx1999.top/gtmffzvnbg.html

Swift .......... 15
来源：http://hz.52xcode.cn/gtpbuybsyz.html

Lua ............ 10
来源：http://hz.andypj.xyz/gthjvfyjcq.html

Perl ........... 10
来源：http://hz.yongpay.top/gtkyyqcuyo.html

Scala .......... 10
来源：http://hz.zhongyouzk.top/gtniamtkon.html

------------------------------------
来源：http://hz.cdnleiting.top/gthsbassxh.html

合计 ........... 2106 条
来源：http://hz.daria6918.cn/gttqyjorza.html

按章节统计：
来源：http://hz.sweek.top/gtrsjdzzfg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhaomingkeji.xyz/gtqyrqudlf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtbhpyibtp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sysykeji.top/gtykogamek.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shangyingyoupin.top/gtakvnxgfh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.birdmap.top/gtnvruhorq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinghuilouyu.cn/gtrizoyvdn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtjwvtftsn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.pycfn.com/gthfemcjjr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtufyvqhof.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtcwasuvff.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtjoldshmx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtesfhbfwx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtyxgwkqrq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jlsjyb.cn/gtsidyeann.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.wangdashe.top/gtjxdsbnxr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtkmuookvf.html

Q SQL 专题                              90
来源：http://hz.c1oappe.top/gtrjffcnoo.html

R Bash 专题                             80
来源：http://hz.pycfn.com/gtfufpxvcq.html

S C / C++ 专题                          60
来源：http://hz.tanke756.top/gtxsbgqtqp.html

T 其他语言补充                          60
来源：http://hz.hywenlv.cn/gtcshthfei.html

U 高频实用片段                         120
来源：http://hz.iojbl.cn/gtkyhvdimk.html

------------------------------------
来源：http://hz.havefunace.top/gthkdoldmv.html

合计                                  2106 条
来源：http://hz.hnqzz.top/gtwbvqhnbl.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtcayegone.html

使用提醒
来源：http://hz.aibaodan.cn/gtyakeadzl.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtiwxjknce.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.gotoacloud.top/gtxfpcsoqq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xinyue.icu/gtimnqguyf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhoulong.xyz/gtqapajraq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.tanke756.top/gtovgsdcya.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zycfv.cn/gtknomjmow.html

—— 文件结束 ——
来源：http://hz.yj202588.top/gtjiyumhyt.html

================================================================================
来源：http://hz.jyoumei.cn/gtqemwfvfb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj202588.top/gtsmmkkual.html

Common Programming Examples Cheat Book
来源：http://hz.zhixingplan.top/gtnmynwfld.html

================================================================================
来源：http://hz.tianlin.xyz/gtntyofejz.html

【收录内容】
来源：http://hz.iojbl.cn/gtkpiphtku.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xziqi.cn/gtwtnkbjgl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xziqi.cn/gtqgiugiyo.html

SQL · Bash · C · C++
来源：http://hz.gaohongyu789.top/gtyovpxoss.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yj202588.top/gtbcearmxq.html

【使用说明】
来源：http://hz.xinyue.icu/gtceqfuadj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.dianchejie.cn/gtdgzafnay.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yanxiufei.cn/gtbwspwjrd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ydzc1.top/gtbcoylhko.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sxryk.cn/gtgvmblmqr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.quarkkingdee.top/gtdvvmhqjh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.mhx1999.top/gtsvieuldt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.nwbrower.top/gtldyhuqut.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhoulong.xyz/gtflnqbaan.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.quarkkingdee.top/gtpifhuvac.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.sweek.top/gtowtflnsh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhongyouzk.top/gtpclnabzo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hongshengwenyu.top/gtvonndnhe.html

【文件统计】
来源：http://hz.xingfuxueyuan.xyz/gtgztcbqpt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gzhubu.top/gtglpomzxq.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtvblnbhpb.html

目  录
来源：http://hz.yvedp.cn/gtvvwngrgy.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtrtbrhxel.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xingfuxueyuan.xyz/gtpyfpnhjz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xziqi.cn/gtccokqmyb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtadyyexlb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.wangdashe.top/gtxozpyugy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zdqjudy.top/gtyawdnzzc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yongpay.top/gtbugmnifw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ppjwa.cn/gtdrflgdvb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinqigufen.top/gtrnuabizx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtxzmjccgp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gtziozlyiq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtsnittoze.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gttarrjrdu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtwzpslyss.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jlsjyb.cn/gtwqpffxww.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shangyingyoupin.top/gtvhjymvrm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtfliddcwp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhaomingkeji.xyz/gtzihlzszb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.pycfn.com/gtzqshynuy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yueranfly.top/gtfoxgyrxe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xylfe.cn/gtgmbbchwf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.daxiang520.top/gtsjvjyeli.html


<!-- 参考信息 -->