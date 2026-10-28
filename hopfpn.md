代发 wailian999

[U19] Py：正则替换带回调
来源：http://hz.zhixingplan.top/gtjznmkmwv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.feifeiyinyue.top/gtmhdjbyeg.html

[U20] Py：缓存函数结果
来源：http://hz.ppjwa.cn/gtouuztktv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.iojbl.cn/gtnghktkvq.html

[U21] Py：自定义上下文管理器
来源：http://hz.birdmap.top/gtggjfpjvh.html

@contextlib.contextmanager
来源：http://hz.ydzc1.top/gtndwzjczd.html

[U22] Py：矩阵转置
来源：http://hz.xuanzx.com/gtiijyrgzg.html

list(zip(*m))
来源：http://hz.cdnleiting.top/gtgnbqtcib.html

[U23] Py：分块读取大文件
来源：http://hz.hfpthk.cn/gtwcqbuzfi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yanxiufei.cn/gtstcttlbc.html

[U24] Py：路径操作
来源：http://hz.jiagoushi.top/gtnxxpiimq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jianghu66.top/gtcsjeeroa.html

[U25] Py：CSV 按字典读
来源：http://hz.haohaochexian.top/gtcjuplmrq.html

csv.DictReader(f)
来源：http://hz.ydzc1.top/gtugbgoojt.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gtjyhukhly.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jinghuilouyu.cn/gtoxapvbhe.html

[U27] Py：异步 HTTP
来源：http://hz.hnqzz.top/gthkdzgmny.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhengqikj.top/gtmrxweoid.html

[U28] Py：类型别名
来源：http://hz.kuanghao11.cn/gtpzevmtnf.html

UserId = int
来源：http://hz.tianlin.xyz/gtrqvegrye.html

[U29] Py：属性校验
来源：http://hz.guannengcc.top/gtxyuhszoi.html

@property 与 @x.setter 配合
来源：http://hz.jianghu66.top/gtvastusdr.html

[U30] Py：数据类
来源：http://hz.shangyingyoupin.top/gtccfncwnr.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gtvoismdre.html

[U31] Py：单测
来源：http://hz.cdnleiting.top/gtwxxzqsjv.html

python -m pytest -q
来源：http://hz.snrcjt.cn/gtjzhupanz.html

[U32] Py：代码格式化
来源：http://hz.chenzaomai.com/gthsmntikg.html

ruff format . && ruff check --fix .
来源：http://hz.guannengcc.top/gtrkpurvnf.html

[U33] Py：打包发布
来源：http://hz.iojbl.cn/gtynvcbkts.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hongshengwenyu.top/gtvvjkuvxm.html

[U34] Py：判断编码
来源：http://hz.gogol.net.cn/gtxvtsduul.html

chardet.detect(raw)
来源：http://hz.ppjwa.cn/gtwyoikzmq.html

[U35] Py：发送邮件
来源：http://hz.tianlin.xyz/gtkdhoiwxy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yanxiufei.cn/gtlogbplqi.html

[U36] Py：定时任务
来源：http://hz.shanyushiyangkeji.top/gtetghdals.html

schedule.every(10).minutes.do(job)
来源：http://hz.mhx1999.top/gtikpbxyxh.html

[U37] Py：读写 Excel
来源：http://hz.tianlin.xyz/gtcfvssarl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhengqikj.top/gtrmbnweiq.html

[U38] Py：获取脚本所在目录
来源：http://hz.daxiang520.top/gtwgxndznc.html

Path(__file__).resolve().parent
来源：http://hz.xinyue.icu/gtoddyxkhd.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhijiandao.cn/gtekyahnki.html

sys.stdout.isatty()
来源：http://hz.aibaodan.cn/gtxusszzna.html

[U40] Py：打印到标准错误
来源：http://hz.nanxinkj.top/gtlqiluktr.html

print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtglohfbnl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yj20258.top/gtqyqhkjor.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.c1oappe.top/gthfxctvjz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinqigufen.top/gtfnsettdu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.feifeiyinyue.top/gtuffjeewa.html

[U43] PHP：声明命名空间
来源：http://hz.tian-w.cn/gtwwrtdsyk.html

namespace App\Http;
来源：http://hz.jqgufenzy.top/gtxjnnsvyp.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangkeji.top/gtcdfrwnbr.html

declare(strict_types=1);
来源：http://hz.yuanzhike.top/gtdeqkhych.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shangyingyoupin.top/gtsxsqgcgy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gtsckwlzdw.html

[U46] PHP：可空类型
来源：http://hz.zhixingplan.top/gtrflvssha.html

?string $name = null
来源：http://hz.sxryk.cn/gtlutnbzem.html

[U47] PHP：联合类型
来源：http://hz.cucudq.cn/gtrstseakc.html

int|string $id
来源：http://hz.shangyingyoupin.top/gtjrpkohib.html

[U48] PHP：纯枚举
来源：http://hz.jiagoushi.top/gtktvtzicm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xylfe.cn/gtybsrlszv.html

[U49] PHP：只读属性
来源：http://hz.jqgfzy.top/gtktfsvgfz.html

public readonly string $name
来源：http://hz.yongpay.top/gttaffxyst.html

[U50] PHP：构造器属性提升
来源：http://hz.bjfxy.top/gtrpcssmmo.html

public function __construct(private int $id) {}
来源：http://hz.shzxlz.cn/gtdwymmajh.html

[U51] PHP：数组解构
来源：http://hz.xuetiantiany.cn/gtwgjatwfg.html

[$a, $b] = $arr;
来源：http://hz.chenzaomai.com/gtgmyevfxg.html

[U52] PHP：箭头函数
来源：http://hz.jyoumei.cn/gtfyqiyxew.html

$double = fn($x) => $x * 2;
来源：http://hz.shanyushiyangkeji.top/gtqxtthkbe.html

[U53] PHP：空合并运算符
来源：http://hz.snrcjt.cn/gtqvciktnf.html

$v = $a ?? $b ?? "default";
来源：http://hz.gogol.net.cn/gtdpnqogpt.html

[U54] PHP：空安全调用
来源：http://hz.yuxming.cn/gtcqzogpsv.html

$obj?->method()
来源：http://hz.yonumen.top/gtdvtkitrl.html

[U55] PHP：match 表达式
来源：http://hz.hfpthk.cn/gtxgwjxrex.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jinyuanbaomall.cn/gtttgeptvq.html

[U56] PHP：命名参数
来源：http://hz.yanxiufei.cn/gtyqkfcjfk.html

f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtqovubtzu.html

[U57] PHP：字符串插值
来源：http://hz.svipenyu.cn/gtdkuiloue.html

"值: {$a}"
来源：http://hz.birdmap.top/gtbsdiqvmd.html

[U58] PHP：数组三件套
来源：http://hz.nanxinkj.top/gtgjlkmvsn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ywan-chungtsiang.top/gtrgucvohe.html

[U59] PHP：自定义排序
来源：http://hz.jqgfzy.top/gtkwktckcz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtfqcsvmtq.html

[U60] PHP：JSON 编解码
来源：http://hz.gzhubu.top/gtjjmcizls.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.wangdashe.top/gtohattoap.html

[U61] PHP：正则
来源：http://hz.dashuyun.cn/gtlmrgmhip.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtpzycsima.html

[U62] PHP：日期对象
来源：http://hz.zhixingplan.top/gtoariiqxn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.pycfn.com/gtlvzjrlki.html

[U63] PHP：文件读写
来源：http://hz.ivvv.top/gtkxqtphdy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258888.top/gtxkzbbhtx.html

[U64] PHP：目录遍历
来源：http://hz.xuetiantiany.cn/gtfdomnxtc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.iojbl.cn/gtghitbczd.html

[U65] PHP：会话
来源：http://hz.hammf.cn/gtlwqhpxnk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xuanzx.com/gtqgqpcqbv.html

[U66] PHP：设置 Cookie
来源：http://hz.zhixingplan.top/gtagujllzg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cqqwz.cn/gtuvhozqdt.html

[U67] PHP：处理文件上传
来源：http://hz.tian-w.cn/gtdesyppik.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenjidiqi.icu/gthdscwidp.html

[U68] PHP：PDO 连接
来源：http://hz.jiagoushi.top/gtdtczgzwk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ywan-chungtsiang.top/gtzkouqzlu.html

[U69] PHP：PDO 预处理
来源：http://hz.ybcxt.top/gtxbpewkca.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jqgufenzy.top/gtmrmtgytx.html

[U70] PHP：PDO 事务
来源：http://hz.zhijiandao.cn/gtppovhuer.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.chenlongwang.top/gtnkduxfdi.html

[U71] PHP：抛出异常
来源：http://hz.yj20258888.top/gtfdnbomjn.html

throw new RuntimeException("失败", 500);
来源：http://hz.9152youxi.cn/gtiqyfpyib.html

[U72] PHP：写错误日志
来源：http://hz.yvedp.cn/gtelvnopfr.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yueranfly.top/gtrvdekape.html

[U73] PHP：读取 ini 配置
来源：http://hz.zycfv.cn/gtcjmfqovl.html

parse_ini_file("config.ini", true)
来源：http://hz.tianlin.xyz/gtmpqqtlih.html

[U74] PHP：读取环境变量
来源：http://hz.zhoulong.xyz/gteijrhgwk.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shanyushiyangtech.top/gtmnjyhoxa.html

[U75] PHP：依赖注入
来源：http://hz.0kj1m.cn/gtspxgrwbx.html

composer require psr/container
来源：http://hz.316326.xyz/gtfjjadabe.html

[U76] PHP：简单路由
来源：http://hz.birdmap.top/gtkkfogria.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.pengpengdd.cyou/gtekutezpo.html

[U77] PHP：模板渲染
来源：http://hz.xuetiantiany.cn/gthxqdynwm.html

composer require twig/twig
来源：http://hz.hysaishi.cn/gtybxjoeie.html

[U78] PHP：单元测试
来源：http://hz.yj20258888.top/gtfxsdazyc.html

composer require --dev phpunit/phpunit
来源：http://hz.tianlin.xyz/gthxrjqkfc.html

[U79] PHP：静态分析
来源：http://hz.nwbrower.top/gtcczwkoht.html

composer require --dev phpstan/phpstan
来源：http://hz.jqgfzy.top/gthvwbohrq.html

[U80] PHP：代码规范修复
来源：http://hz.dashuyun.cn/gtfsfaukzj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.gaohongyu789.top/gtpphznben.html

[U81] JS：初始化项目
来源：http://hz.jyoumei.cn/gtfzyjyhoc.html

npm init -y;  npm i express
来源：http://hz.smart0.xyz/gtovmnsers.html

[U82] JS：package.json 脚本
来源：http://hz.jiagoushi.top/gtiyjmzvpp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yuanzhike.top/gtiwjtyhhg.html

[U83] JS：ES Module 导入导出
来源：http://hz.chenzaomai.com/gtmjhgektu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ivvv.top/gtgnykrvvg.html

[U84] JS：CommonJS 写法
来源：http://hz.cucudq.cn/gtqdiauqli.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangshuangyany.cn/gtatbxlard.html

[U85] JS：可选链
来源：http://hz.9152youxi.cn/gtbhhgoiny.html

a?.b?.c
来源：http://hz.sweek.top/gtntibhgvq.html

[U86] JS：空值合并
来源：http://hz.yvedp.cn/gtsvloqruj.html

a ?? b
来源：http://hz.gotoacloud.top/gtsuazrwmn.html

[U87] JS：解构默认值
来源：http://hz.yj20258.top/gtftjfyswe.html

const { a = 1, b = 2 } = obj;
来源：http://hz.meibo888.top/gtlllnqhyx.html

[U88] JS：对象展开合并
来源：http://hz.tanke756.top/gtgskmkmib.html

{ ...a, ...b }
来源：http://hz.52xcode.cn/gtpjsjmpjc.html

[U89] JS：数组去重
来源：http://hz.yongpay.top/gtbkqfygtq.html

[...new Set(arr)]
来源：http://hz.daria6918.cn/gtvzuflcbf.html

[U90] JS：数字数组排序
来源：http://hz.nanxuanxn.top/gtzwpqywwe.html

[...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtobntilgt.html

[U91] JS：对象键值遍历
来源：http://hz.xuetiantiany.cn/gtecffwobu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.wangshuangyany.cn/gtudtoxmqu.html

[U92] JS：深拷贝
来源：http://hz.jqgfzy.top/gtirvdaucv.html

structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtkbklibxf.html

[U93] JS：模板字符串
来源：http://hz.wangdashe.top/gtogskuxcp.html

`共 ${n} 条`
来源：http://hz.ydjk.org.cn/gtjfqqdxya.html

[U94] JS：箭头函数
来源：http://hz.gogol.net.cn/gtlygfyyxc.html

const double = x => x * 2;
来源：http://hz.yj20258888.top/gtvuqhjuvr.html

[U95] JS：Promise 包装
来源：http://hz.zhiwuduotai.top/gtbjoozzri.html

new Promise((resolve, reject) => {})
来源：http://hz.sweek.top/gtaottaynt.html

[U96] JS：async/await 与异常
来源：http://hz.pycfn.com/gteslmmlwt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigufen.top/gtaqzfakji.html

[U97] JS：并发请求
来源：http://hz.cheryme.top/gtmxlgfyor.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtxbtkarfb.html

[U98] JS：fetch 带 JSON
来源：http://hz.cdnleiting.top/gtlozfxjmo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.haohaochexian.top/gtxovordoz.html

[U99] JS：事件监听
来源：http://hz.jlsjyb.cn/gtitxmuoki.html

el.addEventListener("click", e => {})
来源：http://hz.jianghu66.top/gtjrmaqchv.html

[U100] JS：DOM 查询
来源：http://hz.sweek.top/gtrwwtanoc.html

document.querySelector(".item")
来源：http://hz.yj202588.top/gtqdibynzl.html

[U101] JS：classList 操作
来源：http://hz.gotoacloud.top/gtgjwkleuk.html

el.classList.toggle("active")
来源：http://hz.xingfuxueyuan.xyz/gtkxuiihee.html

[U102] JS：本地存储
来源：http://hz.yvedp.cn/gtzrrumkdj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ywan-chungtsiang.top/gtwtyhnggs.html

[U103] JS：定时器
来源：http://hz.jqgufenzy.top/gtdzfxhvfn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xinyue.icu/gtvoyejrbs.html

[U104] JS：防抖
来源：http://hz.tian-w.cn/gtsbzjbrmn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtpusxdtti.html

[U105] JS：节流
来源：http://hz.zdqjudy.top/gtzaapvgnr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.pengpengdd.cyou/gtmltbiuwv.html

[U106] JS：日期格式化
来源：http://hz.havefunace.top/gtuxmfgzdl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yangfankeji.com/gttcvvylxb.html

[U107] JS：数字千分位
来源：http://hz.daxiang520.top/gtvtsvqpke.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.sysykeji.top/gtwtmvzpng.html

[U108] JS：随机整数
来源：http://hz.jlsjyb.cn/gtzmtdqbbl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.gaohongyu789.top/gtroyoickx.html

[U109] JS：数组分组
来源：http://hz.yj20258.top/gtrpjxeiiq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.pengpengdd.cyou/gtdkeebnot.html

[U110] JS：数组分块
来源：http://hz.redwolf501.top/gtdsbndmtm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yuanzhike.top/gtgxfjjawo.html

[U111] JS：对象转 Map
来源：http://hz.fengsongda.top/gtourzziba.html

new Map(Object.entries(obj))
来源：http://hz.tianlin.xyz/gtlcgvpvkf.html

[U112] JS：字符串补位
来源：http://hz.zhengqikj.top/gtmthqxvjz.html

"7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtjundvury.html

[U113] JS：正则替换全部
来源：http://hz.zdqjudy.top/gtqgezxidk.html

s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtfbwpxojs.html

[U114] JS：JSON 深比较
来源：http://hz.ydzc1.top/gtwnfaxfbp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gthvohaigc.html

[U115] JS：生成 UUID
来源：http://hz.tianlin.xyz/gtufzsiiwu.html

crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtyslxgovz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xinyue.icu/gtvvxlsxxo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.nanxuanxn.top/gtzvnrfgmh.html

[U117] JS：单元测试
来源：http://hz.jqgfzy.top/gtrbkllkbt.html

npm i -D vitest;  npx vitest
来源：http://hz.zhixingplan.top/gtwmubjean.html

[U118] JS：开发服务器
来源：http://hz.guowangkeji.top/gtwvpbwrxm.html

npm i -D vite;  npx vite
来源：http://hz.daxiang520.top/gtqcakdkph.html

[U119] JS：生产构建
来源：http://hz.xziqi.cn/gtvnjmpqiy.html

npx vite build
来源：http://hz.sxryk.cn/gtflrwzmft.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yueranfly.top/gtecibhvqe.html

import.meta.env.VITE_API_URL
来源：http://hz.ydjk.org.cn/gteeklpczx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gteyksxwaj.html

统计汇总
来源：http://hz.sufxvd.cn/gtysxclotr.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfvkvbjwg.html

按语言统计（条）：
来源：http://hz.yuanzhike.top/gthbbfroxc.html

Python ......... 252
来源：http://hz.xuetiantiany.cn/gtplfhnjiu.html

PHP ............ 252
来源：http://hz.jinghuilouyu.cn/gtftprczck.html

JavaScript ..... 252
来源：http://hz.daxiang520.top/gtcdnxwkuc.html

TypeScript ..... 212
来源：http://hz.jiagoushi.top/gtuulanixk.html

Java ........... 212
来源：http://hz.sweek.top/gtzybxwnfv.html

Go ............. 212
来源：http://hz.yangfankeji.com/gtsgnfsckx.html

Ruby ........... 212
来源：http://hz.hammf.cn/gtjzkpkwmr.html

C# ............. 212
来源：http://hz.yonumen.top/gtisbciciy.html

C .............. 30
来源：http://hz.ydzc1.top/gtigrpcfvn.html

C++ ............ 30
来源：http://hz.zhaomingkeji.xyz/gtexaaskyr.html

SQL ............ 90
来源：http://hz.gogol.net.cn/gtxcchmedx.html

Bash ........... 80
来源：http://hz.yonumen.top/gtlqoaadjh.html

Kotlin ......... 15
来源：http://hz.sufxvd.cn/gtyibdhmaj.html

Swift .......... 15
来源：http://hz.sufxvd.cn/gtsmibietq.html

Lua ............ 10
来源：http://hz.yongpay.top/gtridimuvx.html

Perl ........... 10
来源：http://hz.cheryme.top/gtchpqtxli.html

Scala .......... 10
来源：http://hz.bjfxy.top/gtsvlbntzj.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtzcwgjklr.html

合计 ........... 2106 条
来源：http://hz.feifeiyinyue.top/gtjmqxrcmx.html

按章节统计：
来源：http://hz.aibaodan.cn/gtgvicbluo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinqigfzy.top/gtiwfxcjnu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtxsuldija.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtmwldmvry.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hfpthk.cn/gtjyaspjbs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xinyue.icu/gtmcqumjfe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jyoumei.cn/gtsinghbdw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtrznxkkdz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtimktkbra.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtswniyhlj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtumklrznb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtvfvewyop.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gthradgvsz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtzfttmhcv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.dianchejie.cn/gtrrknenqq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.meibo888.top/gtixzzwzfn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtkzipywrf.html

Q SQL 专题                              90
来源：http://hz.sweek.top/gtoljfyefw.html

R Bash 专题                             80
来源：http://hz.gaohongyu789.top/gtpbbkxohq.html

S C / C++ 专题                          60
来源：http://hz.haohaochexian.top/gtlrhwborv.html

T 其他语言补充                          60
来源：http://hz.c1oappe.top/gtuifnvyyw.html

U 高频实用片段                         120
来源：http://hz.jlsjyb.cn/gtygaqispo.html

------------------------------------
来源：http://hz.ybcxt.top/gtotwpevdj.html

合计                                  2106 条
来源：http://hz.yongpay.top/gtbzbplnnr.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtzygatpdm.html

使用提醒
来源：http://hz.havefunace.top/gtyxrxjvwb.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gtjhvfrcji.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.pycfn.com/gtvevzemkz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.gaohongyu789.top/gtalevitrm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.nanxinkj.top/gteqhjzhky.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yueranfly.top/gtvhxwdjio.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hnqzz.top/gtxtekqjim.html

—— 文件结束 ——
来源：http://hz.shuidangran.top/gteetsgahi.html

================================================================================
来源：http://hz.dianchejie.cn/gtcwuttggp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hfpthk.cn/gtfiyndvqj.html

Common Programming Examples Cheat Book
来源：http://hz.xinyue.icu/gtykrcazkk.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtglfmmdlp.html

【收录内容】
来源：http://hz.sufxvd.cn/gtzuzqmfmz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj20258888.top/gtqkgnjklb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yuanzhike.top/gtckbpqhty.html

SQL · Bash · C · C++
来源：http://hz.nanxinkj.top/gtvwhhzbge.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.chenlongwang.top/gthoomcisk.html

【使用说明】
来源：http://hz.tianlin.xyz/gtuvcmpyxn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yueranfly.top/gtcwdracvw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shzxlz.cn/gtgnxamwbg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj202588.top/gtgvwgryqk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cheryme.top/gtmjtijasg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhoulong.xyz/gtrpckqsyy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jinqigfzy.top/gtnkcplrrm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hnqzz.top/gtowmemyfa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jinqigfzy.top/gtvulunbty.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yanxiufei.cn/gthmtoxblo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhoulong.xyz/gtydeeaeeg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.cucudq.cn/gtikafojwt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hnxiangtu.top/gtyeawresv.html

【文件统计】
来源：http://hz.hnxiangtu.top/gtxcahrvkg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.daxiang520.top/gtsgeovnlx.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gtnkiwbzqc.html

目  录
来源：http://hz.ydjk.org.cn/gtthicahrp.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gteicvokiq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jinqigufen.top/gthcnoojln.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gtbvrohfnw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ehwqpu.com/gtrvvgleek.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sufxvd.cn/gtwghvrinm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shangyingyoupin.top/gtzynburra.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenlongwang.top/gtrctnhpdh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtixunbtql.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.c1oappe.top/gtjvnjdhtr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtahxrkgwk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ywan-chungtsiang.top/gthuhtlpti.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtiliilzbx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gtajbewbto.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtsgxjuukq.html


<!-- 参考信息 -->