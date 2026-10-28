代发 wailian999

[U17] Py：初始化日志
来源：http://hz.jqgufenzy.top/gtsgowjqcw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.guowangkeji.top/gtibrarici.html

[U18] Py：预编译正则
来源：http://hz.andypj.xyz/gtxlgjorra.html

pat = re.compile(r"\d+")
来源：http://hz.chenlongwang.top/gtdxuwhvgv.html

[U19] Py：正则替换带回调
来源：http://hz.xuetiantiany.cn/gtvuffukzl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.snrcjt.cn/gtvndfajge.html

[U20] Py：缓存函数结果
来源：http://hz.shanyushiyangkeji.top/gtkliisnun.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ehwqpu.com/gtcshmmfie.html

[U21] Py：自定义上下文管理器
来源：http://hz.52xcode.cn/gtrufwyjfd.html

@contextlib.contextmanager
来源：http://hz.zdqjudy.top/gtxqpotakv.html

[U22] Py：矩阵转置
来源：http://hz.yangfankeji.com/gtqypgghse.html

list(zip(*m))
来源：http://hz.316326.xyz/gtpattvqsq.html

[U23] Py：分块读取大文件
来源：http://hz.haohaochexian.top/gtpdlfsqwj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zdqjudy.top/gtyhzoaeye.html

[U24] Py：路径操作
来源：http://hz.xziqi.cn/gtbxbdjslf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxuanxn.top/gtpobxnahy.html

[U25] Py：CSV 按字典读
来源：http://hz.gaohongyu789.top/gtjiswqhsg.html

csv.DictReader(f)
来源：http://hz.hammf.cn/gtxgoranec.html

[U26] Py：并发下载
来源：http://hz.jiagoushi.top/gtdwrazgmk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ydzc1.top/gtzteudeuu.html

[U27] Py：异步 HTTP
来源：http://hz.zhijiandao.cn/gtuxcypvtl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhijiandao.cn/gtrdpsefps.html

[U28] Py：类型别名
来源：http://hz.quarkkingdee.top/gtdaujgoan.html

UserId = int
来源：http://hz.ehwqpu.com/gtcviafhks.html

[U29] Py：属性校验
来源：http://hz.xinyue.icu/gtgnjteovn.html

@property 与 @x.setter 配合
来源：http://hz.yuanzhike.top/gtfyljcgic.html

[U30] Py：数据类
来源：http://hz.quarkkingdee.top/gtwagkrptx.html

@dataclass(slots=True)
来源：http://hz.c1oappe.top/gtwaxqahuz.html

[U31] Py：单测
来源：http://hz.wangdashe.top/gtejnijydi.html

python -m pytest -q
来源：http://hz.yueranfly.top/gtpulrfoel.html

[U32] Py：代码格式化
来源：http://hz.sysykeji.top/gtmjmwtmpl.html

ruff format . && ruff check --fix .
来源：http://hz.ydzc1.top/gtacscfqai.html

[U33] Py：打包发布
来源：http://hz.gogol.net.cn/gttukutfrq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.meibo888.top/gtayupgwzg.html

[U34] Py：判断编码
来源：http://hz.sysykeji.top/gtkkgrglam.html

chardet.detect(raw)
来源：http://hz.guowangkeji.top/gtjefqflra.html

[U35] Py：发送邮件
来源：http://hz.yueranfly.top/gtzjjqwlal.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zdqjudy.top/gtbfcnofyz.html

[U36] Py：定时任务
来源：http://hz.tianlin.xyz/gtkqzxinsa.html

schedule.every(10).minutes.do(job)
来源：http://hz.ppjwa.cn/gtmkdfyrpt.html

[U37] Py：读写 Excel
来源：http://hz.yvedp.cn/gtquaqvbap.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.feifeiyinyue.top/gtznlczbuk.html

[U38] Py：获取脚本所在目录
来源：http://hz.xingfuxueyuan.xyz/gtbhunjaqv.html

Path(__file__).resolve().parent
来源：http://hz.yuanzhike.top/gtxzrwkkml.html

[U39] Py：判断是否在交互环境
来源：http://hz.zycfv.cn/gtoizozjzg.html

sys.stdout.isatty()
来源：http://hz.jqgufenzy.top/gtejwvhucd.html

[U40] Py：打印到标准错误
来源：http://hz.fengsongda.top/gtmkuokljm.html

print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtumzqtmhm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.daxiang520.top/gtirsloehg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sufxvd.cn/gtvuprrhif.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenjidiqi.icu/gtgqgdlwds.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.iojbl.cn/gtdcscyaoc.html

[U43] PHP：声明命名空间
来源：http://hz.cqqwz.cn/gtbkimkkoy.html

namespace App\Http;
来源：http://hz.ybcxt.top/gturgayiag.html

[U44] PHP：开启严格类型
来源：http://hz.sufxvd.cn/gtvwfxkitf.html

declare(strict_types=1);
来源：http://hz.sweek.top/gtzkdvmhea.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhijiandao.cn/gtfeuudyem.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxuanxn.top/gtnuweigne.html

[U46] PHP：可空类型
来源：http://hz.guannengcc.top/gtobliozoj.html

?string $name = null
来源：http://hz.ywan-chungtsiang.top/gtdfzmddgv.html

[U47] PHP：联合类型
来源：http://hz.hfpthk.cn/gtkfnnjaqw.html

int|string $id
来源：http://hz.shangyingyoupin.top/gthywdbsjd.html

[U48] PHP：纯枚举
来源：http://hz.guowangkeji.top/gtrzlxqcoc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.mhx1999.top/gtvdcjgteb.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gtlhaaiduu.html

public readonly string $name
来源：http://hz.yj202588.top/gtbxgfotzf.html

[U50] PHP：构造器属性提升
来源：http://hz.cdnleiting.top/gtyxjldbuf.html

public function __construct(private int $id) {}
来源：http://hz.yonumen.top/gtjmdvtvhm.html

[U51] PHP：数组解构
来源：http://hz.xylfe.cn/gtlzikbahh.html

[$a, $b] = $arr;
来源：http://hz.tian-w.cn/gtvoyurhzf.html

[U52] PHP：箭头函数
来源：http://hz.cashguo.top/gtfensyvzz.html

$double = fn($x) => $x * 2;
来源：http://hz.daria6918.cn/gtznrlzfyc.html

[U53] PHP：空合并运算符
来源：http://hz.yangfankeji.com/gtkyccxjet.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhaomingkeji.xyz/gtosmgurjm.html

[U54] PHP：空安全调用
来源：http://hz.c1oappe.top/gtvxlhzbro.html

$obj?->method()
来源：http://hz.jqgfzy.top/gtciehqtsg.html

[U55] PHP：match 表达式
来源：http://hz.ehwqpu.com/gtelcxsnad.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jlsjyb.cn/gtajaxafuh.html

[U56] PHP：命名参数
来源：http://hz.jinqigfzy.top/gtercuisfx.html

f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtwfftddbt.html

[U57] PHP：字符串插值
来源：http://hz.cheryme.top/gttmtwlkbs.html

"值: {$a}"
来源：http://hz.cucudq.cn/gtdmucyoxl.html

[U58] PHP：数组三件套
来源：http://hz.snrcjt.cn/gtltobjndy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenzaomai.com/gthwdixpks.html

[U59] PHP：自定义排序
来源：http://hz.svipenyu.cn/gtoanhohtj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daria6918.cn/gtsbzysrwl.html

[U60] PHP：JSON 编解码
来源：http://hz.xziqi.cn/gtoamvokzr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guowangkeji.top/gtrywphnut.html

[U61] PHP：正则
来源：http://hz.gzhubu.top/gtpkebtdpn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtpsgfcgvy.html

[U62] PHP：日期对象
来源：http://hz.ydjk.org.cn/gtcuwvwmam.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.iojbl.cn/gturnnmzpg.html

[U63] PHP：文件读写
来源：http://hz.snrcjt.cn/gtpcfahxwu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sysykeji.top/gtgzjegxvg.html

[U64] PHP：目录遍历
来源：http://hz.ydzc1.top/gtvrqgsdfk.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yongpay.top/gtpuzrzvlc.html

[U65] PHP：会话
来源：http://hz.zhengqikj.top/gtcnlpddwc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhixingplan.top/gtxfenjfgn.html

[U66] PHP：设置 Cookie
来源：http://hz.yj202588.top/gtzqutfplw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.dashuyun.cn/gtibbpvjgw.html

[U67] PHP：处理文件上传
来源：http://hz.yuanzhike.top/gtlgoqtxve.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xuetiantiany.cn/gtvwqrpyif.html

[U68] PHP：PDO 连接
来源：http://hz.wangdashe.top/gtgewqsoxn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ywan-chungtsiang.top/gtdhwkkezn.html

[U69] PHP：PDO 预处理
来源：http://hz.guowangkeji.top/gtgxcsblmz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yvedp.cn/gtdpiqssnl.html

[U70] PHP：PDO 事务
来源：http://hz.hnqzz.top/gteetwnuwk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gogol.net.cn/gtrafphcop.html

[U71] PHP：抛出异常
来源：http://hz.sysykeji.top/gtiasdztwh.html

throw new RuntimeException("失败", 500);
来源：http://hz.xuetiantiany.cn/gtnianjein.html

[U72] PHP：写错误日志
来源：http://hz.jqgfzy.top/gtcuhssktm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.svipenyu.cn/gteklckqjf.html

[U73] PHP：读取 ini 配置
来源：http://hz.0kj1m.cn/gtsfgupadg.html

parse_ini_file("config.ini", true)
来源：http://hz.cucudq.cn/gtaknzfjgv.html

[U74] PHP：读取环境变量
来源：http://hz.hywenlv.cn/gtgaohmhfc.html

getenv("APP_ENV") ?: "production"
来源：http://hz.bjfxy.top/gtvhuarevw.html

[U75] PHP：依赖注入
来源：http://hz.zhongyouzk.top/gtykyvwwwb.html

composer require psr/container
来源：http://hz.hywenlv.cn/gtieneukzs.html

[U76] PHP：简单路由
来源：http://hz.hywenlv.cn/gtaifqxbac.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jinqigfzy.top/gtgblpgikf.html

[U77] PHP：模板渲染
来源：http://hz.hammf.cn/gtafjphoic.html

composer require twig/twig
来源：http://hz.sxryk.cn/gtnyfvobuj.html

[U78] PHP：单元测试
来源：http://hz.hfpthk.cn/gtokfgbban.html

composer require --dev phpunit/phpunit
来源：http://hz.zhiwuduotai.top/gtmvoazovh.html

[U79] PHP：静态分析
来源：http://hz.316326.xyz/gtvspuxryt.html

composer require --dev phpstan/phpstan
来源：http://hz.nanxinkj.top/gttnbzlasx.html

[U80] PHP：代码规范修复
来源：http://hz.yangfankeji.com/gtxfbqigkw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xylfe.cn/gtvspbtzfa.html

[U81] JS：初始化项目
来源：http://hz.hongshengwenyu.top/gttkpqeknl.html

npm init -y;  npm i express
来源：http://hz.chenjidiqi.icu/gtyzcqwjdt.html

[U82] JS：package.json 脚本
来源：http://hz.sufxvd.cn/gtumngnhdz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.fengsongda.top/gtblecnjmn.html

[U83] JS：ES Module 导入导出
来源：http://hz.ywan-chungtsiang.top/gtqgpiwhho.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ehwqpu.com/gtbzrpulky.html

[U84] JS：CommonJS 写法
来源：http://hz.c1oappe.top/gtsmoylrzg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.birdmap.top/gtwqbjujoz.html

[U85] JS：可选链
来源：http://hz.iojbl.cn/gtfemwkjoa.html

a?.b?.c
来源：http://hz.hywenlv.cn/gtmhuxuycu.html

[U86] JS：空值合并
来源：http://hz.vqdsnc.cn/gtvmmdimbk.html

a ?? b
来源：http://hz.hywenlv.cn/gtrbsqrsjn.html

[U87] JS：解构默认值
来源：http://hz.316326.xyz/gtgirtaxce.html

const { a = 1, b = 2 } = obj;
来源：http://hz.iojbl.cn/gtfpqrjjut.html

[U88] JS：对象展开合并
来源：http://hz.hnxiangtu.top/gtkupvswjt.html

{ ...a, ...b }
来源：http://hz.ydjk.org.cn/gtfeeovrus.html

[U89] JS：数组去重
来源：http://hz.aizwys.cn/gtlkstpolb.html

[...new Set(arr)]
来源：http://hz.zycfv.cn/gtoqkgmxxg.html

[U90] JS：数字数组排序
来源：http://hz.chenjidiqi.icu/gtaqnvfnis.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtgevspltz.html

[U91] JS：对象键值遍历
来源：http://hz.bjfxy.top/gtetfpymuv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yongpay.top/gttghxhjzt.html

[U92] JS：深拷贝
来源：http://hz.redwolf501.top/gtcqunedym.html

structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtjehttzcg.html

[U93] JS：模板字符串
来源：http://hz.fzhhl.top/gtqrcgkhqp.html

`共 ${n} 条`
来源：http://hz.guannengcc.top/gttefjughn.html

[U94] JS：箭头函数
来源：http://hz.guowangkeji.top/gtsyghccge.html

const double = x => x * 2;
来源：http://hz.daria6918.cn/gtehrswdmq.html

[U95] JS：Promise 包装
来源：http://hz.hysaishi.cn/gtweltuunu.html

new Promise((resolve, reject) => {})
来源：http://hz.jinqigufen.top/gtpaqpjtvu.html

[U96] JS：async/await 与异常
来源：http://hz.yangfankeji.com/gtnudrxjbk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtlfcxolqc.html

[U97] JS：并发请求
来源：http://hz.yj20258888.top/gtmpmsoqor.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtcqfgttfz.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhengqikj.top/gtxwqmpubg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.fzhhl.top/gtxfohrlcl.html

[U99] JS：事件监听
来源：http://hz.316326.xyz/gtevlkgmym.html

el.addEventListener("click", e => {})
来源：http://hz.shanyushiyangtech.top/gtokfvzgqi.html

[U100] JS：DOM 查询
来源：http://hz.hnqzz.top/gtmsvxqiss.html

document.querySelector(".item")
来源：http://hz.gzhubu.top/gtapnicutn.html

[U101] JS：classList 操作
来源：http://hz.ybcxt.top/gtvvstbkft.html

el.classList.toggle("active")
来源：http://hz.jianghu66.top/gtlhmvzhpr.html

[U102] JS：本地存储
来源：http://hz.vqdsnc.cn/gtieljmiyr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xuanzx.com/gtguehqnib.html

[U103] JS：定时器
来源：http://hz.cucudq.cn/gtldjuzoje.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.nwbrower.top/gtgmtdtaan.html

[U104] JS：防抖
来源：http://hz.chenzaomai.com/gtvhfohixn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtvqjuzvsf.html

[U105] JS：节流
来源：http://hz.hfpthk.cn/gthpmibvto.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuxming.cn/gtmqtkqwtz.html

[U106] JS：日期格式化
来源：http://hz.nwbrower.top/gtlgqtxpzc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinqigfzy.top/gthaiotngc.html

[U107] JS：数字千分位
来源：http://hz.haohaochexian.top/gttchrgiqk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tanke756.top/gtmoxhdogl.html

[U108] JS：随机整数
来源：http://hz.zdqjudy.top/gtglaclklp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cashguo.top/gthftvinko.html

[U109] JS：数组分组
来源：http://hz.cashguo.top/gtpzbmmnyz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhaomingkeji.xyz/gtnqagayxs.html

[U110] JS：数组分块
来源：http://hz.yuxming.cn/gtzdfvsgxl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ybcxt.top/gthuylcmht.html

[U111] JS：对象转 Map
来源：http://hz.mhx1999.top/gtnbtnrrdo.html

new Map(Object.entries(obj))
来源：http://hz.yvedp.cn/gtizlxfikh.html

[U112] JS：字符串补位
来源：http://hz.xinyue.icu/gtpqwlbfsr.html

"7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtxupisoji.html

[U113] JS：正则替换全部
来源：http://hz.hongshengwenyu.top/gtaqkzczba.html

s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtntwjgssh.html

[U114] JS：JSON 深比较
来源：http://hz.svipenyu.cn/gtdxyrnqhy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cqqwz.cn/gtesucqkoo.html

[U115] JS：生成 UUID
来源：http://hz.havefunace.top/gtivzhyucm.html

crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtyeiwfmzs.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guowangkeji.top/gthujjwtoq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gotoacloud.top/gtnovckhxo.html

[U117] JS：单元测试
来源：http://hz.sweek.top/gtzpjftpih.html

npm i -D vitest;  npx vitest
来源：http://hz.cqqwz.cn/gtucsudfnj.html

[U118] JS：开发服务器
来源：http://hz.bjfxy.top/gtjesnychw.html

npm i -D vite;  npx vite
来源：http://hz.tianlin.xyz/gtcctublgf.html

[U119] JS：生产构建
来源：http://hz.ehwqpu.com/gtcccvckmg.html

npx vite build
来源：http://hz.shanyushiyangkeji.top/gtahrltbsd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gotoacloud.top/gtkchrfpng.html

import.meta.env.VITE_API_URL
来源：http://hz.hysaishi.cn/gtpzhaksyy.html

================================================================================
来源：http://hz.vqdsnc.cn/gtuawyrrwc.html

统计汇总
来源：http://hz.zhiwuduotai.top/gtqabranqc.html

================================================================================
来源：http://hz.hywenlv.cn/gtlsndcvzq.html

按语言统计（条）：
来源：http://hz.cqqwz.cn/gtzhkzwwgp.html

Python ......... 252
来源：http://hz.dianchejie.cn/gtjspqxvrw.html

PHP ............ 252
来源：http://hz.zycfv.cn/gtboetljsw.html

JavaScript ..... 252
来源：http://hz.xuetiantiany.cn/gtxrhxkrna.html

TypeScript ..... 212
来源：http://hz.shuidangran.top/gtjaklsvpl.html

Java ........... 212
来源：http://hz.jqgufenzy.top/gtpityxvwq.html

Go ............. 212
来源：http://hz.zycfv.cn/gtbaehidvp.html

Ruby ........... 212
来源：http://hz.pycfn.com/gtlrhcuums.html

C# ............. 212
来源：http://hz.shanyushiyangtech.top/gtdqdkzscx.html

C .............. 30
来源：http://hz.kuanghao11.cn/gtezolirfp.html

C++ ............ 30
来源：http://hz.chenjidiqi.icu/gtzzyxasro.html

SQL ............ 90
来源：http://hz.0kj1m.cn/gtiiqsfuta.html

Bash ........... 80
来源：http://hz.cucudq.cn/gtxsztevdi.html

Kotlin ......... 15
来源：http://hz.jinyuanbaomall.cn/gttygqjuxk.html

Swift .......... 15
来源：http://hz.ydjk.org.cn/gtytevnwos.html

Lua ............ 10
来源：http://hz.jyoumei.cn/gtgppstrmd.html

Perl ........... 10
来源：http://hz.kuanghao11.cn/gtsikpbapo.html

Scala .......... 10
来源：http://hz.guowangkeji.top/gtetzauctk.html

------------------------------------
来源：http://hz.yangfankeji.com/gtamsyfvkg.html

合计 ........... 2106 条
来源：http://hz.chenjidiqi.icu/gtkxmyrdmc.html

按章节统计：
来源：http://hz.ybcxt.top/gtyemdkxqd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.c1oappe.top/gtuhlkenpw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gtfhuxgusd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sxryk.cn/gtpmrnmbnh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinghuilouyu.cn/gtzyrgmjcf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yj20258888.top/gtsqxdawvi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jiagoushi.top/gtrwjsduii.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtbpypmjto.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.pengpengdd.cyou/gtahtqvnim.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gtnmvdwfwx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhixingplan.top/gtvwdixflo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtoapjptai.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtxgngjjpl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gttjzuxfvt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj202588.top/gtimuiviem.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.guannengcc.top/gtvoyocakq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gttsjfbton.html

Q SQL 专题                              90
来源：http://hz.xziqi.cn/gtibodivbh.html

R Bash 专题                             80
来源：http://hz.shangyingyoupin.top/gtyrukickd.html

S C / C++ 专题                          60
来源：http://hz.jqgufenzy.top/gterujrqvv.html

T 其他语言补充                          60
来源：http://hz.daxiang520.top/gtwsbkleum.html

U 高频实用片段                         120
来源：http://hz.sufxvd.cn/gtgvioncde.html

------------------------------------
来源：http://hz.yj20258.top/gtdvltqafn.html

合计                                  2106 条
来源：http://hz.jqgfzy.top/gtcrroxucd.html

--------------------------------------------------------------------------------
来源：http://hz.yongpay.top/gttcjdaeum.html

使用提醒
来源：http://hz.xingfuxueyuan.xyz/gtmvwyxtzj.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtrbortdon.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhiwuduotai.top/gtyixsqjpw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ppjwa.cn/gtehgibwjo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.andypj.xyz/gtsquiyfih.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.fzhhl.top/gtqnxrqbjk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ppjwa.cn/gtearkwdho.html

—— 文件结束 ——
来源：http://hz.wangdashe.top/gthwdvowgm.html

================================================================================
来源：http://hz.nwbrower.top/gttahtmlkc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.bjfxy.top/gtnptxqadf.html

Common Programming Examples Cheat Book
来源：http://hz.jqgfzy.top/gtnucdtmpw.html

================================================================================
来源：http://hz.haohaochexian.top/gtxeswvdfv.html

【收录内容】
来源：http://hz.hnqzz.top/gtkewyhezo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhiwuduotai.top/gtvbrrzlyf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.vqdsnc.cn/gtfphmrrij.html

SQL · Bash · C · C++
来源：http://hz.yuxming.cn/gtmeswyqkj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.quarkkingdee.top/gtyxmqktwv.html

【使用说明】
来源：http://hz.ivvv.top/gtuxbvjhfy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.quarkkingdee.top/gtkgsjucif.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ydzc1.top/gtiavxcfgo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258888.top/gtdasdbtrc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jinyuanbaomall.cn/gtvijypcpu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gzhubu.top/gtsmozsxcp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.pycfn.com/gtetjqrvhm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yongpay.top/gtfyyxoouu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yueranfly.top/gtzyggfltf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nanxinkj.top/gtnmeqquno.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yj202588.top/gtzyysdhiw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.snrcjt.cn/gtvwhkjohw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ydjk.org.cn/gttaqzxxjn.html

【文件统计】
来源：http://hz.xinyue.icu/gtahkypqzd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.daria6918.cn/gtyotwdbab.html

--------------------------------------------------------------------------------
来源：http://hz.tianlin.xyz/gtwtppfmjs.html

目  录
来源：http://hz.gotoacloud.top/gtjzwswgpc.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtadsxjrij.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.havefunace.top/gtppoaqoeo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ppjwa.cn/gtelauecgj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xylfe.cn/gtoucelqkn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhixingplan.top/gtwgktzhkf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jiagoushi.top/gtrwawrfnu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ppjwa.cn/gtieeqhddk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gtodwjgqwh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yonumen.top/gtriiprzjv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xinyue.icu/gtarthdduj.html


<!-- 参考信息 -->