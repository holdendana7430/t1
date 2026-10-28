代发 wailian999

[U15] Py：高精度计时
来源：http://hz.nanxinkj.top/gtykffwuym.html

t = time.perf_counter()
来源：http://hz.wangdashe.top/gtfvrummxi.html

[U16] Py：命令行参数解析
来源：http://hz.zhengqikj.top/gtzlbvrljg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nwbrower.top/gtrqetweif.html

[U17] Py：初始化日志
来源：http://hz.zhoulong.xyz/gtqzkoaxnm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sweek.top/gtxeipjniv.html

[U18] Py：预编译正则
来源：http://hz.jinghuilouyu.cn/gtmfigxjlv.html

pat = re.compile(r"\d+")
来源：http://hz.zdqjudy.top/gtswkutzdj.html

[U19] Py：正则替换带回调
来源：http://hz.xuetiantiany.cn/gtmwnnaast.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.snrcjt.cn/gtszfdkhtu.html

[U20] Py：缓存函数结果
来源：http://hz.cashguo.top/gtjwnlroxt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.svipenyu.cn/gtwpzsenmh.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhongyouzk.top/gtpawjvnsp.html

@contextlib.contextmanager
来源：http://hz.shanyushiyangkeji.top/gtkbegquxi.html

[U22] Py：矩阵转置
来源：http://hz.cucudq.cn/gtwofbdofa.html

list(zip(*m))
来源：http://hz.xuetiantiany.cn/gtnwhcwecb.html

[U23] Py：分块读取大文件
来源：http://hz.cashguo.top/gtoyssqhgl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xuanzx.com/gtdbkhobcg.html

[U24] Py：路径操作
来源：http://hz.sufxvd.cn/gtqlsazolw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.feifeiyinyue.top/gteexqfhpb.html

[U25] Py：CSV 按字典读
来源：http://hz.ydjk.org.cn/gtcdtruxlq.html

csv.DictReader(f)
来源：http://hz.zycfv.cn/gtyqchgzif.html

[U26] Py：并发下载
来源：http://hz.bjfxy.top/gtcufbcbzj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jianghu66.top/gtexzhxwyy.html

[U27] Py：异步 HTTP
来源：http://hz.hammf.cn/gthflywjcq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.316326.xyz/gtyzhwoipw.html

[U28] Py：类型别名
来源：http://hz.ppjwa.cn/gthqojdpyv.html

UserId = int
来源：http://hz.shanyushiyangkeji.top/gtzhevglim.html

[U29] Py：属性校验
来源：http://hz.316326.xyz/gteebadlgw.html

@property 与 @x.setter 配合
来源：http://hz.aibaodan.cn/gtwsqhejci.html

[U30] Py：数据类
来源：http://hz.iojbl.cn/gtgbmcjcqo.html

@dataclass(slots=True)
来源：http://hz.tanke756.top/gtzzfvgyvg.html

[U31] Py：单测
来源：http://hz.c1oappe.top/gtzubwdxta.html

python -m pytest -q
来源：http://hz.gzhubu.top/gtxkkruxij.html

[U32] Py：代码格式化
来源：http://hz.ybcxt.top/gtvsujdcxj.html

ruff format . && ruff check --fix .
来源：http://hz.iojbl.cn/gtxrpdqiqe.html

[U33] Py：打包发布
来源：http://hz.zhoulong.xyz/gtaupgavea.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yonumen.top/gtmnoqjior.html

[U34] Py：判断编码
来源：http://hz.kuanghao11.cn/gtkberxpzy.html

chardet.detect(raw)
来源：http://hz.gogol.net.cn/gtnidgnzwd.html

[U35] Py：发送邮件
来源：http://hz.guannengcc.top/gtrehpadwo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yuxming.cn/gtbbeystyu.html

[U36] Py：定时任务
来源：http://hz.dashuyun.cn/gtidsytskb.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhongyouzk.top/gtrdkxvysx.html

[U37] Py：读写 Excel
来源：http://hz.cucudq.cn/gttetfeogc.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shuidangran.top/gtypfnvfct.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxuanxn.top/gtupemsnvg.html

Path(__file__).resolve().parent
来源：http://hz.gzhubu.top/gtgiofceak.html

[U39] Py：判断是否在交互环境
来源：http://hz.cucudq.cn/gtcynxaetf.html

sys.stdout.isatty()
来源：http://hz.yangfankeji.com/gtkyjvvbiq.html

[U40] Py：打印到标准错误
来源：http://hz.nanxinkj.top/gtdpgjhqzs.html

print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtuasgdqqy.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gaohongyu789.top/gtpqmjmknf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yj20258.top/gtcomjlivm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hnqzz.top/gtqlzllttp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xuanzx.com/gtplxyizeq.html

[U43] PHP：声明命名空间
来源：http://hz.ehwqpu.com/gtbnypkmat.html

namespace App\Http;
来源：http://hz.aibaodan.cn/gteivejvpl.html

[U44] PHP：开启严格类型
来源：http://hz.cucudq.cn/gtvcgvsixp.html

declare(strict_types=1);
来源：http://hz.wangdashe.top/gtccvbgsnz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jinqigufen.top/gtaxlrozcc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cashguo.top/gtgzzudigo.html

[U46] PHP：可空类型
来源：http://hz.nanxuanxn.top/gtxtgzbgcc.html

?string $name = null
来源：http://hz.52xcode.cn/gtjdmadsqb.html

[U47] PHP：联合类型
来源：http://hz.9152youxi.cn/gtnntsygep.html

int|string $id
来源：http://hz.haohaochexian.top/gtxlrxmaic.html

[U48] PHP：纯枚举
来源：http://hz.sweek.top/gtxxfxkehg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tanke756.top/gtcexthrjk.html

[U49] PHP：只读属性
来源：http://hz.yvedp.cn/gtvmuguxql.html

public readonly string $name
来源：http://hz.ydzc1.top/gtgeafcuzf.html

[U50] PHP：构造器属性提升
来源：http://hz.zycfv.cn/gtfohjhujl.html

public function __construct(private int $id) {}
来源：http://hz.chenzaomai.com/gtzjqgjnyb.html

[U51] PHP：数组解构
来源：http://hz.ivvv.top/gtuhnmtnzk.html

[$a, $b] = $arr;
来源：http://hz.nanxinkj.top/gtyilrcpxg.html

[U52] PHP：箭头函数
来源：http://hz.yueranfly.top/gtgkwqgzir.html

$double = fn($x) => $x * 2;
来源：http://hz.fengsongda.top/gthoygpxdi.html

[U53] PHP：空合并运算符
来源：http://hz.sysykeji.top/gtpxltlcmr.html

$v = $a ?? $b ?? "default";
来源：http://hz.guannengcc.top/gtjcieoere.html

[U54] PHP：空安全调用
来源：http://hz.jlsjyb.cn/gtpcsqbmlr.html

$obj?->method()
来源：http://hz.9152youxi.cn/gtqohnvtxp.html

[U55] PHP：match 表达式
来源：http://hz.tian-w.cn/gtsdgfqcmr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ehwqpu.com/gtwhkplphd.html

[U56] PHP：命名参数
来源：http://hz.tianlin.xyz/gtcblwcnrk.html

f(a: 1, b: 2)
来源：http://hz.haohaochexian.top/gtflnposfo.html

[U57] PHP：字符串插值
来源：http://hz.tian-w.cn/gtngvhvpbv.html

"值: {$a}"
来源：http://hz.hfpthk.cn/gtzlgniyty.html

[U58] PHP：数组三件套
来源：http://hz.gzhubu.top/gtiyjgszeq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.snrcjt.cn/gtvjqskjkz.html

[U59] PHP：自定义排序
来源：http://hz.guowangkeji.top/gtmtwoampe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtsgopecyj.html

[U60] PHP：JSON 编解码
来源：http://hz.0kj1m.cn/gtcorozjsm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cheryme.top/gtjvfpuhqz.html

[U61] PHP：正则
来源：http://hz.wangshuangyany.cn/gttmjzmdcd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.fzhhl.top/gtqbxmczhx.html

[U62] PHP：日期对象
来源：http://hz.yangfankeji.com/gtqlhwyawz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gotoacloud.top/gthxingcjy.html

[U63] PHP：文件读写
来源：http://hz.nanxuanxn.top/gtndjyrqkn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shzxlz.cn/gtvukcjryg.html

[U64] PHP：目录遍历
来源：http://hz.jqgfzy.top/gtfunijrhu.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.guowangkeji.top/gtarzlybhe.html

[U65] PHP：会话
来源：http://hz.shanyushiyangtech.top/gtcwzilpas.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ydjk.org.cn/gtqlebfwpp.html

[U66] PHP：设置 Cookie
来源：http://hz.yueranfly.top/gtjfgniphb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.9152youxi.cn/gtyuemgeew.html

[U67] PHP：处理文件上传
来源：http://hz.jinghuilouyu.cn/gtmvmiocvd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hnxiangtu.top/gtawslxsyk.html

[U68] PHP：PDO 连接
来源：http://hz.yonumen.top/gtxcwewwce.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenjidiqi.icu/gtsqwfnafw.html

[U69] PHP：PDO 预处理
来源：http://hz.xingfuxueyuan.xyz/gtvaxzjims.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.pengpengdd.cyou/gtfbbswqll.html

[U70] PHP：PDO 事务
来源：http://hz.zhiwuduotai.top/gtlkreczwz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sweek.top/gtppvzzhxt.html

[U71] PHP：抛出异常
来源：http://hz.shanyushiyangtech.top/gtvbfsxvvg.html

throw new RuntimeException("失败", 500);
来源：http://hz.yonumen.top/gtzikrfcgo.html

[U72] PHP：写错误日志
来源：http://hz.kuanghao11.cn/gtevsbzozr.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jinqigufen.top/gtfybsrflh.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydzc1.top/gtuzqwcfeb.html

parse_ini_file("config.ini", true)
来源：http://hz.guowangkeji.top/gtwraohbjm.html

[U74] PHP：读取环境变量
来源：http://hz.yongpay.top/gtnrbqlvml.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinqigfzy.top/gthmvpvjol.html

[U75] PHP：依赖注入
来源：http://hz.ppjwa.cn/gtwbodhnhh.html

composer require psr/container
来源：http://hz.redwolf501.top/gtezdfezeb.html

[U76] PHP：简单路由
来源：http://hz.quarkkingdee.top/gtgjrskslt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cashguo.top/gtekcbvkts.html

[U77] PHP：模板渲染
来源：http://hz.jinqigufen.top/gtbxsfcaie.html

composer require twig/twig
来源：http://hz.smart0.xyz/gtugefpysi.html

[U78] PHP：单元测试
来源：http://hz.jiagoushi.top/gtcxzbkjgt.html

composer require --dev phpunit/phpunit
来源：http://hz.xuetiantiany.cn/gtyrbxrmok.html

[U79] PHP：静态分析
来源：http://hz.pycfn.com/gtyuqgakiu.html

composer require --dev phpstan/phpstan
来源：http://hz.aizwys.cn/gthqbgdnlo.html

[U80] PHP：代码规范修复
来源：http://hz.dashuyun.cn/gtvfvpwkrc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zdqjudy.top/gtiiaelhue.html

[U81] JS：初始化项目
来源：http://hz.xziqi.cn/gtlahdcduc.html

npm init -y;  npm i express
来源：http://hz.chenzaomai.com/gtygqkiqgi.html

[U82] JS：package.json 脚本
来源：http://hz.zhijiandao.cn/gtbveufiin.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xinyue.icu/gtgfgmmrfm.html

[U83] JS：ES Module 导入导出
来源：http://hz.guowangkeji.top/gttraukoye.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xingfuxueyuan.xyz/gtsydbfxdn.html

[U84] JS：CommonJS 写法
来源：http://hz.zhijiandao.cn/gturkknihg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinqigfzy.top/gthbcftxkb.html

[U85] JS：可选链
来源：http://hz.shuidangran.top/gtlycpwriv.html

a?.b?.c
来源：http://hz.iojbl.cn/gtniulqwdc.html

[U86] JS：空值合并
来源：http://hz.snrcjt.cn/gtrbaqirqw.html

a ?? b
来源：http://hz.nanxuanxn.top/gtunekvusd.html

[U87] JS：解构默认值
来源：http://hz.yvedp.cn/gtipaisqnk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhongyouzk.top/gtnokesqko.html

[U88] JS：对象展开合并
来源：http://hz.hnqzz.top/gtteqiaflq.html

{ ...a, ...b }
来源：http://hz.cashguo.top/gtbldixqsf.html

[U89] JS：数组去重
来源：http://hz.0kj1m.cn/gtrdkevhwb.html

[...new Set(arr)]
来源：http://hz.ydzc1.top/gtbpzxerto.html

[U90] JS：数字数组排序
来源：http://hz.yonumen.top/gthmwsbdhd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtexqwdtpa.html

[U91] JS：对象键值遍历
来源：http://hz.ydzc1.top/gtvrlynibu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.9152youxi.cn/gtmzfnzqwy.html

[U92] JS：深拷贝
来源：http://hz.yuanzhike.top/gtvnuijqlv.html

structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtctglxtcx.html

[U93] JS：模板字符串
来源：http://hz.sufxvd.cn/gtbhveolbh.html

`共 ${n} 条`
来源：http://hz.sxryk.cn/gttpxlbamv.html

[U94] JS：箭头函数
来源：http://hz.tian-w.cn/gtdrmxikey.html

const double = x => x * 2;
来源：http://hz.sysykeji.top/gtcpmaastt.html

[U95] JS：Promise 包装
来源：http://hz.snrcjt.cn/gtpdlgzfkc.html

new Promise((resolve, reject) => {})
来源：http://hz.xuanzx.com/gtgndnyria.html

[U96] JS：async/await 与异常
来源：http://hz.9152youxi.cn/gtutpubcqa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtdsigutzw.html

[U97] JS：并发请求
来源：http://hz.xinyue.icu/gtqendmshx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtmonstpaz.html

[U98] JS：fetch 带 JSON
来源：http://hz.cqqwz.cn/gtwvhmznav.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ehwqpu.com/gtbqzimldw.html

[U99] JS：事件监听
来源：http://hz.hnqzz.top/gtdfplludr.html

el.addEventListener("click", e => {})
来源：http://hz.9152youxi.cn/gtzfcljyqx.html

[U100] JS：DOM 查询
来源：http://hz.yanxiufei.cn/gtqgbccrki.html

document.querySelector(".item")
来源：http://hz.daria6918.cn/gtpmofabbo.html

[U101] JS：classList 操作
来源：http://hz.gaohongyu789.top/gtjxunzong.html

el.classList.toggle("active")
来源：http://hz.ehwqpu.com/gtjngaboaw.html

[U102] JS：本地存储
来源：http://hz.ehwqpu.com/gtcdpvbjyz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yanxiufei.cn/gtmcsflhib.html

[U103] JS：定时器
来源：http://hz.shzxlz.cn/gtlppbvopx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.kuanghao11.cn/gtcggjaiua.html

[U104] JS：防抖
来源：http://hz.0kj1m.cn/gtehuvnuib.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtfkolxczq.html

[U105] JS：节流
来源：http://hz.zdqjudy.top/gtlngwxpef.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ydjk.org.cn/gtvtdguvtv.html

[U106] JS：日期格式化
来源：http://hz.iojbl.cn/gtxjvnpdpk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.birdmap.top/gtkqqstcpy.html

[U107] JS：数字千分位
来源：http://hz.hysaishi.cn/gtpldgtyqn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.pengpengdd.cyou/gtxbeanigj.html

[U108] JS：随机整数
来源：http://hz.jlsjyb.cn/gtfhrzimfd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tianlin.xyz/gtopfrohoz.html

[U109] JS：数组分组
来源：http://hz.cheryme.top/gtojzkpjee.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jqgfzy.top/gtdtffeuhv.html

[U110] JS：数组分块
来源：http://hz.tanke756.top/gtwywjjtlw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cdnleiting.top/gtgcmsxtom.html

[U111] JS：对象转 Map
来源：http://hz.ywan-chungtsiang.top/gtkgaafanb.html

new Map(Object.entries(obj))
来源：http://hz.shangyingyoupin.top/gtxuqbzjzh.html

[U112] JS：字符串补位
来源：http://hz.yangfankeji.com/gtlbpuruet.html

"7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtysserczf.html

[U113] JS：正则替换全部
来源：http://hz.shuidangran.top/gthiyqvsmf.html

s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtipnljkmf.html

[U114] JS：JSON 深比较
来源：http://hz.fengsongda.top/gtoguawfak.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtncszupuc.html

[U115] JS：生成 UUID
来源：http://hz.fengsongda.top/gtiufuafuz.html

crypto.randomUUID()
来源：http://hz.c1oappe.top/gtshkcznfg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.redwolf501.top/gttzhwszvo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yonumen.top/gtqzwvnvvx.html

[U117] JS：单元测试
来源：http://hz.nanxinkj.top/gttwjztvfr.html

npm i -D vitest;  npx vitest
来源：http://hz.zhoulong.xyz/gttwbhektm.html

[U118] JS：开发服务器
来源：http://hz.daxiang520.top/gtbzkyiheb.html

npm i -D vite;  npx vite
来源：http://hz.gzhubu.top/gtomgmvhia.html

[U119] JS：生产构建
来源：http://hz.nanxinkj.top/gtvavouamd.html

npx vite build
来源：http://hz.yj20258.top/gtfiyglbmx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.dashuyun.cn/gtvxawdqql.html

import.meta.env.VITE_API_URL
来源：http://hz.316326.xyz/gtyzxwcjqm.html

================================================================================
来源：http://hz.sxryk.cn/gtzqkirsfq.html

统计汇总
来源：http://hz.jinqigufen.top/gtkfmvjofv.html

================================================================================
来源：http://hz.tian-w.cn/gtuyozmxvs.html

按语言统计（条）：
来源：http://hz.yanxiufei.cn/gtwjcdxgph.html

Python ......... 252
来源：http://hz.cashguo.top/gtyfykbicf.html

PHP ............ 252
来源：http://hz.dashuyun.cn/gtvmqhihip.html

JavaScript ..... 252
来源：http://hz.zycfv.cn/gtrwkvfilu.html

TypeScript ..... 212
来源：http://hz.sysykeji.top/gtjbjmzbvp.html

Java ........... 212
来源：http://hz.hnxiangtu.top/gtmomxyfym.html

Go ............. 212
来源：http://hz.zhengqikj.top/gtqqjyxjml.html

Ruby ........... 212
来源：http://hz.gaohongyu789.top/gtpntnevbd.html

C# ............. 212
来源：http://hz.gogol.net.cn/gtbnoqqyow.html

C .............. 30
来源：http://hz.xuanzx.com/gtipnhagaf.html

C++ ............ 30
来源：http://hz.yuxming.cn/gtholppufe.html

SQL ............ 90
来源：http://hz.yanxiufei.cn/gtnnhqslmq.html

Bash ........... 80
来源：http://hz.chenlongwang.top/gthjjiqhdg.html

Kotlin ......... 15
来源：http://hz.zhiwuduotai.top/gtqykkzlbi.html

Swift .......... 15
来源：http://hz.gotoacloud.top/gtxenmpbgx.html

Lua ............ 10
来源：http://hz.zhengqikj.top/gtumnyatho.html

Perl ........... 10
来源：http://hz.ehwqpu.com/gtidrclviz.html

Scala .......... 10
来源：http://hz.snrcjt.cn/gtmegiwppu.html

------------------------------------
来源：http://hz.cheryme.top/gtmrleooxq.html

合计 ........... 2106 条
来源：http://hz.hammf.cn/gtiqevsnak.html

按章节统计：
来源：http://hz.yongpay.top/gtrqzlzcrl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jiagoushi.top/gtnrvxjvxk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yonumen.top/gtpqfcwsuv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtzvfleyss.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.dianchejie.cn/gtqhtthinp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hywenlv.cn/gtjtdmvnwc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zycfv.cn/gtcysbsite.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtdcbvvxhx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yonumen.top/gtayqzzzik.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtwlbllhcc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hammf.cn/gtqlsogyms.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtffxyolck.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtigqlwqfw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtacakmhry.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.daria6918.cn/gtzonlbsse.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.redwolf501.top/gtjfypylkz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gthmuyldou.html

Q SQL 专题                              90
来源：http://hz.gaohongyu789.top/gtpupakmoo.html

R Bash 专题                             80
来源：http://hz.haohaochexian.top/gtjlozcbxj.html

S C / C++ 专题                          60
来源：http://hz.hammf.cn/gtvvznmfut.html

T 其他语言补充                          60
来源：http://hz.yj202588.top/gtizmqaikr.html

U 高频实用片段                         120
来源：http://hz.yangfankeji.com/gthkypapop.html

------------------------------------
来源：http://hz.zdqjudy.top/gtbipsabob.html

合计                                  2106 条
来源：http://hz.xuetiantiany.cn/gtunzqavdm.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtarbnkcow.html

使用提醒
来源：http://hz.ydjk.org.cn/gttgicxcro.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gtbhbqwrsp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shuidangran.top/gtfkniekur.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinghuilouyu.cn/gtrymkdytl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.aibaodan.cn/gtcowrqcdp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.smart0.xyz/gtrkuhvvoq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aibaodan.cn/gtzmurozcy.html

—— 文件结束 ——
来源：http://hz.0kj1m.cn/gtmbdghsnp.html

================================================================================
来源：http://hz.yonumen.top/gtrzvenpab.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ydzc1.top/gtszvyhqwt.html

Common Programming Examples Cheat Book
来源：http://hz.yvedp.cn/gtczrmqzgf.html

================================================================================
来源：http://hz.hywenlv.cn/gtqkgvgxql.html

【收录内容】
来源：http://hz.xinyue.icu/gthlaauxly.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ybcxt.top/gtcxydwvne.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.sweek.top/gtzkxnrzan.html

SQL · Bash · C · C++
来源：http://hz.yueranfly.top/gtfafwgbet.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hongshengwenyu.top/gttgujngzi.html

【使用说明】
来源：http://hz.9152youxi.cn/gtbuiabubp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ybcxt.top/gtngajdcfd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tianlin.xyz/gtpnqpmnxg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jqgufenzy.top/gtdglryraf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhixingplan.top/gtstfqtafp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhongyouzk.top/gtgntrmool.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.dianchejie.cn/gtmgkuiubd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yangfankeji.com/gteycnmrrq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.haohaochexian.top/gtjkrkrlpf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.pengpengdd.cyou/gtqbfoybqa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.fzhhl.top/gtbiitwuda.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yanxiufei.cn/gtbnngklbi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.52xcode.cn/gttpkpetis.html

【文件统计】
来源：http://hz.xinyue.icu/gtnhdqxodm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ppjwa.cn/gtsinsiknu.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtlrioprdy.html

目  录
来源：http://hz.shanyushiyangkeji.top/gtdpqtizwl.html

--------------------------------------------------------------------------------
来源：http://hz.fengsongda.top/gtkzcxjakl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yuxming.cn/gtopqyyumf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cheryme.top/gtvjyvxwut.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.svipenyu.cn/gtgkqtibmr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.smart0.xyz/gtqahvrsoq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cashguo.top/gtzgdfytjc.html


<!-- 参考信息 -->