代发 wailian999

[U13] Py：固定长度队列
来源：http://hz.tanke756.top/gtushsxmop.html

deque(maxlen=10)
来源：http://hz.zdqjudy.top/gtnuqladtu.html

[U14] Py：分组收集到列表
来源：http://hz.wangshuangyany.cn/gthadclzeh.html

defaultdict(list)
来源：http://hz.c1oappe.top/gtrpnykmhv.html

[U15] Py：高精度计时
来源：http://hz.zhaomingkeji.xyz/gtnqxirwrb.html

t = time.perf_counter()
来源：http://hz.pycfn.com/gtegocrkow.html

[U16] Py：命令行参数解析
来源：http://hz.cheryme.top/gtlgtsropb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jyoumei.cn/gtgvawtmyi.html

[U17] Py：初始化日志
来源：http://hz.sweek.top/gtlgcociho.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hysaishi.cn/gtdmjdmkuu.html

[U18] Py：预编译正则
来源：http://hz.hammf.cn/gtfxxfltal.html

pat = re.compile(r"\d+")
来源：http://hz.hongshengwenyu.top/gtpufccxib.html

[U19] Py：正则替换带回调
来源：http://hz.zhijiandao.cn/gtkftnbvdl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xinyue.icu/gtkigwzujp.html

[U20] Py：缓存函数结果
来源：http://hz.sxryk.cn/gtdlhzyltj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangdashe.top/gtfoykugsb.html

[U21] Py：自定义上下文管理器
来源：http://hz.sufxvd.cn/gtenvyntls.html

@contextlib.contextmanager
来源：http://hz.cdnleiting.top/gtbkmedujm.html

[U22] Py：矩阵转置
来源：http://hz.yj202588.top/gtladafonh.html

list(zip(*m))
来源：http://hz.zhaomingkeji.xyz/gtvtifhhuh.html

[U23] Py：分块读取大文件
来源：http://hz.xingfuxueyuan.xyz/gtupecpnxc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhengqikj.top/gtwzkmorlb.html

[U24] Py：路径操作
来源：http://hz.gogol.net.cn/gtezivqqcz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gotoacloud.top/gtzowwuidv.html

[U25] Py：CSV 按字典读
来源：http://hz.ywan-chungtsiang.top/gtvsyasged.html

csv.DictReader(f)
来源：http://hz.zdqjudy.top/gtsbegekmc.html

[U26] Py：并发下载
来源：http://hz.ehwqpu.com/gtoxuapitg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.redwolf501.top/gtgnmusypg.html

[U27] Py：异步 HTTP
来源：http://hz.xuanzx.com/gthccumlve.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenzaomai.com/gtdcaxtied.html

[U28] Py：类型别名
来源：http://hz.hysaishi.cn/gtggfjkqvu.html

UserId = int
来源：http://hz.xylfe.cn/gthzfoswpu.html

[U29] Py：属性校验
来源：http://hz.shanyushiyangtech.top/gtejpdygqk.html

@property 与 @x.setter 配合
来源：http://hz.ivvv.top/gtixiexguw.html

[U30] Py：数据类
来源：http://hz.yangfankeji.com/gtqnlpjwgw.html

@dataclass(slots=True)
来源：http://hz.wangdashe.top/gtcuhfpoyg.html

[U31] Py：单测
来源：http://hz.chenlongwang.top/gtjfahnril.html

python -m pytest -q
来源：http://hz.shzxlz.cn/gtdpkykgdl.html

[U32] Py：代码格式化
来源：http://hz.nanxuanxn.top/gtnfwldwbe.html

ruff format . && ruff check --fix .
来源：http://hz.jianghu66.top/gtlfvnogzi.html

[U33] Py：打包发布
来源：http://hz.tian-w.cn/gttunrpgxc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ivvv.top/gtazqlmddk.html

[U34] Py：判断编码
来源：http://hz.gotoacloud.top/gtoggifnyh.html

chardet.detect(raw)
来源：http://hz.yuxming.cn/gtlkddothp.html

[U35] Py：发送邮件
来源：http://hz.52xcode.cn/gtjvffvlla.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.dashuyun.cn/gtljcwaspu.html

[U36] Py：定时任务
来源：http://hz.yangfankeji.com/gtregsnalk.html

schedule.every(10).minutes.do(job)
来源：http://hz.zdqjudy.top/gtlclefvku.html

[U37] Py：读写 Excel
来源：http://hz.guannengcc.top/gtxouriqja.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yangfankeji.com/gtvuozwijf.html

[U38] Py：获取脚本所在目录
来源：http://hz.iojbl.cn/gtjurpptwh.html

Path(__file__).resolve().parent
来源：http://hz.c1oappe.top/gtlxxyilqg.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gtdzzzaatb.html

sys.stdout.isatty()
来源：http://hz.jqgufenzy.top/gtknyibpid.html

[U40] Py：打印到标准错误
来源：http://hz.mhx1999.top/gtjqwwguep.html

print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtfebilelc.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shangyingyoupin.top/gtcqrluhya.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gotoacloud.top/gtiwxsuapa.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shanyushiyangtech.top/gtwxyrdvsb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shanyushiyangtech.top/gtlrhfsvgc.html

[U43] PHP：声明命名空间
来源：http://hz.jinyuanbaomall.cn/gtsgdqvuhm.html

namespace App\Http;
来源：http://hz.nanxuanxn.top/gtrzoneniu.html

[U44] PHP：开启严格类型
来源：http://hz.jlsjyb.cn/gtkpgcvbbd.html

declare(strict_types=1);
来源：http://hz.jqgfzy.top/gtawnqqscm.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cqqwz.cn/gtrahzoabx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtoibaayzx.html

[U46] PHP：可空类型
来源：http://hz.yongpay.top/gtroscpbkv.html

?string $name = null
来源：http://hz.ehwqpu.com/gtduhvcflm.html

[U47] PHP：联合类型
来源：http://hz.cashguo.top/gtmefeqwyj.html

int|string $id
来源：http://hz.zhiwuduotai.top/gthehwcweq.html

[U48] PHP：纯枚举
来源：http://hz.ybcxt.top/gtmetscafc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.guannengcc.top/gtszsixfqd.html

[U49] PHP：只读属性
来源：http://hz.kuanghao11.cn/gtgilqckkn.html

public readonly string $name
来源：http://hz.snrcjt.cn/gtseouedfz.html

[U50] PHP：构造器属性提升
来源：http://hz.cucudq.cn/gtqtjsjqhj.html

public function __construct(private int $id) {}
来源：http://hz.jiagoushi.top/gtabktpmbc.html

[U51] PHP：数组解构
来源：http://hz.cdnleiting.top/gtkjobmsgf.html

[$a, $b] = $arr;
来源：http://hz.aizwys.cn/gtgebghykm.html

[U52] PHP：箭头函数
来源：http://hz.jinghuilouyu.cn/gteaemljte.html

$double = fn($x) => $x * 2;
来源：http://hz.c1oappe.top/gtbdhfcvia.html

[U53] PHP：空合并运算符
来源：http://hz.svipenyu.cn/gtrvkmhvvw.html

$v = $a ?? $b ?? "default";
来源：http://hz.yj20258.top/gtlrrzwjib.html

[U54] PHP：空安全调用
来源：http://hz.cqqwz.cn/gtjcfxbxmo.html

$obj?->method()
来源：http://hz.sufxvd.cn/gtkgnnwfne.html

[U55] PHP：match 表达式
来源：http://hz.feifeiyinyue.top/gtqepgyzjw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ywan-chungtsiang.top/gthfnbgrvb.html

[U56] PHP：命名参数
来源：http://hz.dashuyun.cn/gtvvqzsiyw.html

f(a: 1, b: 2)
来源：http://hz.zhijiandao.cn/gtmvcrsdpi.html

[U57] PHP：字符串插值
来源：http://hz.andypj.xyz/gtzalinnqh.html

"值: {$a}"
来源：http://hz.ppjwa.cn/gtndakiarz.html

[U58] PHP：数组三件套
来源：http://hz.vqdsnc.cn/gtinlqmufq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.aizwys.cn/gtlzghldpk.html

[U59] PHP：自定义排序
来源：http://hz.jyoumei.cn/gtnomtmkkd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtysogrkdw.html

[U60] PHP：JSON 编解码
来源：http://hz.andypj.xyz/gtildcgzhp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydzc1.top/gtxirnspoe.html

[U61] PHP：正则
来源：http://hz.jiagoushi.top/gtlggbuqaq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtnfgdgtpr.html

[U62] PHP：日期对象
来源：http://hz.316326.xyz/gtysbomwlt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.daxiang520.top/gtroicbtbt.html

[U63] PHP：文件读写
来源：http://hz.sxryk.cn/gtalpjzifw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.pycfn.com/gtficrvkcj.html

[U64] PHP：目录遍历
来源：http://hz.hammf.cn/gthzmrupue.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yueranfly.top/gtnsigzzfc.html

[U65] PHP：会话
来源：http://hz.chenlongwang.top/gtyieudakc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.0kj1m.cn/gtxtaxrqep.html

[U66] PHP：设置 Cookie
来源：http://hz.shzxlz.cn/gtvcnhpgwz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinqigufen.top/gtpdmdghjk.html

[U67] PHP：处理文件上传
来源：http://hz.jqgfzy.top/gtjrcpbymj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.dianchejie.cn/gtkjcsjfvd.html

[U68] PHP：PDO 连接
来源：http://hz.chenlongwang.top/gtjybidpjf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.daria6918.cn/gtffeeiuaz.html

[U69] PHP：PDO 预处理
来源：http://hz.0kj1m.cn/gtwietomqz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hywenlv.cn/gtnenqaznd.html

[U70] PHP：PDO 事务
来源：http://hz.ybcxt.top/gtputrttee.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gotoacloud.top/gtadhixbgq.html

[U71] PHP：抛出异常
来源：http://hz.guowangkeji.top/gtsccswoko.html

throw new RuntimeException("失败", 500);
来源：http://hz.hysaishi.cn/gtpnxkcphc.html

[U72] PHP：写错误日志
来源：http://hz.jinghuilouyu.cn/gtnxfwbcuv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cqqwz.cn/gtbnccsjct.html

[U73] PHP：读取 ini 配置
来源：http://hz.fengsongda.top/gthzvrxdkr.html

parse_ini_file("config.ini", true)
来源：http://hz.jlsjyb.cn/gtrgsrpmll.html

[U74] PHP：读取环境变量
来源：http://hz.nanxuanxn.top/gtldgskxdh.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenzaomai.com/gtiarmeenw.html

[U75] PHP：依赖注入
来源：http://hz.cdnleiting.top/gtbpocblts.html

composer require psr/container
来源：http://hz.wangshuangyany.cn/gtkgiujzjd.html

[U76] PHP：简单路由
来源：http://hz.gogol.net.cn/gtypghmscj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.redwolf501.top/gtyobxlipi.html

[U77] PHP：模板渲染
来源：http://hz.ivvv.top/gtxaymgdog.html

composer require twig/twig
来源：http://hz.sysykeji.top/gtoqfiamwo.html

[U78] PHP：单元测试
来源：http://hz.yj20258.top/gtggcizzbd.html

composer require --dev phpunit/phpunit
来源：http://hz.feifeiyinyue.top/gtilztmegg.html

[U79] PHP：静态分析
来源：http://hz.jianghu66.top/gtmhfeutxn.html

composer require --dev phpstan/phpstan
来源：http://hz.yongpay.top/gtwctfmydo.html

[U80] PHP：代码规范修复
来源：http://hz.wangshuangyany.cn/gthqbgqucd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sweek.top/gtvbobacla.html

[U81] JS：初始化项目
来源：http://hz.ppjwa.cn/gtrrtxvtvl.html

npm init -y;  npm i express
来源：http://hz.guannengcc.top/gtxnyadcav.html

[U82] JS：package.json 脚本
来源：http://hz.cucudq.cn/gtyxdofhaf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yuxming.cn/gtdieyypuv.html

[U83] JS：ES Module 导入导出
来源：http://hz.tian-w.cn/gtxssnpclu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.daria6918.cn/gtuwpmegfp.html

[U84] JS：CommonJS 写法
来源：http://hz.xinyue.icu/gtzgpozsnu.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.snrcjt.cn/gtijlazlme.html

[U85] JS：可选链
来源：http://hz.fzhhl.top/gtxuzqibph.html

a?.b?.c
来源：http://hz.ivvv.top/gtnvmyelze.html

[U86] JS：空值合并
来源：http://hz.sysykeji.top/gtfuliemor.html

a ?? b
来源：http://hz.chenjidiqi.icu/gtftlbhqav.html

[U87] JS：解构默认值
来源：http://hz.cdnleiting.top/gtozumjqvu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.daxiang520.top/gtuphyvmio.html

[U88] JS：对象展开合并
来源：http://hz.ybcxt.top/gttduftnyp.html

{ ...a, ...b }
来源：http://hz.0kj1m.cn/gtdqqebrnf.html

[U89] JS：数组去重
来源：http://hz.pycfn.com/gtxtifxwfe.html

[...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtjbsvwaro.html

[U90] JS：数字数组排序
来源：http://hz.tanke756.top/gtqzzcnwff.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtlrxrmyti.html

[U91] JS：对象键值遍历
来源：http://hz.andypj.xyz/gtksrkzmac.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zycfv.cn/gtzlpvfgjq.html

[U92] JS：深拷贝
来源：http://hz.jqgufenzy.top/gtbltobdlb.html

structuredClone(obj)
来源：http://hz.yj202588.top/gtsdjaxtgw.html

[U93] JS：模板字符串
来源：http://hz.0kj1m.cn/gtmvhhgcvn.html

`共 ${n} 条`
来源：http://hz.zhaomingkeji.xyz/gtzryhxmbn.html

[U94] JS：箭头函数
来源：http://hz.birdmap.top/gtcctedqel.html

const double = x => x * 2;
来源：http://hz.zhongyouzk.top/gtiiqqhouf.html

[U95] JS：Promise 包装
来源：http://hz.fzhhl.top/gtmdlpgcxq.html

new Promise((resolve, reject) => {})
来源：http://hz.c1oappe.top/gtwpspgjkl.html

[U96] JS：async/await 与异常
来源：http://hz.hysaishi.cn/gtwnxibsvz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtrhqaynfz.html

[U97] JS：并发请求
来源：http://hz.hysaishi.cn/gtnzqdglyx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtbwhberms.html

[U98] JS：fetch 带 JSON
来源：http://hz.cucudq.cn/gtpfopwjpl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jinghuilouyu.cn/gtmozipxey.html

[U99] JS：事件监听
来源：http://hz.yj202588.top/gtqlputgbr.html

el.addEventListener("click", e => {})
来源：http://hz.sweek.top/gtmfickuhk.html

[U100] JS：DOM 查询
来源：http://hz.bjfxy.top/gtndghzzrx.html

document.querySelector(".item")
来源：http://hz.gogol.net.cn/gtwugnzxgz.html

[U101] JS：classList 操作
来源：http://hz.meibo888.top/gtklbpvnwd.html

el.classList.toggle("active")
来源：http://hz.jqgfzy.top/gtzatahnlu.html

[U102] JS：本地存储
来源：http://hz.xuetiantiany.cn/gtofnxmsym.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zdqjudy.top/gtymnnzkxv.html

[U103] JS：定时器
来源：http://hz.316326.xyz/gtbrgeqcrn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinqigufen.top/gtsuchhkhq.html

[U104] JS：防抖
来源：http://hz.chenzaomai.com/gtmlblozad.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtxiqtfhyl.html

[U105] JS：节流
来源：http://hz.cheryme.top/gtwjmfwnbj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gaohongyu789.top/gtadqkkmzi.html

[U106] JS：日期格式化
来源：http://hz.daxiang520.top/gtvrcwokvg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.vqdsnc.cn/gttopgtoop.html

[U107] JS：数字千分位
来源：http://hz.ybcxt.top/gtazjmgiwb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxinkj.top/gtjnagvfhp.html

[U108] JS：随机整数
来源：http://hz.hammf.cn/gtmauyelnm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.vqdsnc.cn/gtjicenwfl.html

[U109] JS：数组分组
来源：http://hz.hnxiangtu.top/gtvnvebgmg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtjrhvlpls.html

[U110] JS：数组分块
来源：http://hz.ywan-chungtsiang.top/gtdgaqzvkb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.52xcode.cn/gtqdavrqpb.html

[U111] JS：对象转 Map
来源：http://hz.shuidangran.top/gtidvlbcae.html

new Map(Object.entries(obj))
来源：http://hz.zhijiandao.cn/gtszuelkng.html

[U112] JS：字符串补位
来源：http://hz.cdnleiting.top/gtceznqasq.html

"7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtgpacqlit.html

[U113] JS：正则替换全部
来源：http://hz.zhijiandao.cn/gtcqxhcxuh.html

s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtjxqksdwx.html

[U114] JS：JSON 深比较
来源：http://hz.gotoacloud.top/gtxjvszjrj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtkojtamge.html

[U115] JS：生成 UUID
来源：http://hz.wangdashe.top/gtplhtynfs.html

crypto.randomUUID()
来源：http://hz.havefunace.top/gtfoojxxsd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.aibaodan.cn/gtagqtojqo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigufen.top/gtsbxgjbhm.html

[U117] JS：单元测试
来源：http://hz.yuanzhike.top/gtnshydxle.html

npm i -D vitest;  npx vitest
来源：http://hz.hongshengwenyu.top/gttqjnqdvo.html

[U118] JS：开发服务器
来源：http://hz.nwbrower.top/gtqmmsdazm.html

npm i -D vite;  npx vite
来源：http://hz.chenjidiqi.icu/gtpgafqvbb.html

[U119] JS：生产构建
来源：http://hz.zycfv.cn/gtieobbkcp.html

npx vite build
来源：http://hz.yanxiufei.cn/gteipacucw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xuetiantiany.cn/gtdcbyxzlc.html

import.meta.env.VITE_API_URL
来源：http://hz.zhengqikj.top/gtlgdgcrue.html

================================================================================
来源：http://hz.gotoacloud.top/gtozhlcbtu.html

统计汇总
来源：http://hz.haohaochexian.top/gtzzwvjrox.html

================================================================================
来源：http://hz.wangdashe.top/gtkttlxyrm.html

按语言统计（条）：
来源：http://hz.ppjwa.cn/gtyeyyjphc.html

Python ......... 252
来源：http://hz.wangdashe.top/gtzvyuqopo.html

PHP ............ 252
来源：http://hz.meibo888.top/gthnljplei.html

JavaScript ..... 252
来源：http://hz.shangyingyoupin.top/gtbnyyhcmw.html

TypeScript ..... 212
来源：http://hz.sysykeji.top/gttkrmqkmk.html

Java ........... 212
来源：http://hz.0kj1m.cn/gtnsctiygu.html

Go ............. 212
来源：http://hz.zhixingplan.top/gtpoyrkuwd.html

Ruby ........... 212
来源：http://hz.yvedp.cn/gtgjjotxyx.html

C# ............. 212
来源：http://hz.pengpengdd.cyou/gtsuygyiqi.html

C .............. 30
来源：http://hz.hnqzz.top/gterqasaal.html

C++ ............ 30
来源：http://hz.haohaochexian.top/gtkbfgptyl.html

SQL ............ 90
来源：http://hz.zhengqikj.top/gtkcznonrj.html

Bash ........... 80
来源：http://hz.pengpengdd.cyou/gthmwaeqam.html

Kotlin ......... 15
来源：http://hz.hongshengwenyu.top/gtgjgdicoj.html

Swift .......... 15
来源：http://hz.shanyushiyangtech.top/gtkaxhxsrh.html

Lua ............ 10
来源：http://hz.jinghuilouyu.cn/gthjrcxgjy.html

Perl ........... 10
来源：http://hz.shuidangran.top/gtluqzkcrm.html

Scala .......... 10
来源：http://hz.jinyuanbaomall.cn/gtexdgywdm.html

------------------------------------
来源：http://hz.yuanzhike.top/gtgrphakcj.html

合计 ........... 2106 条
来源：http://hz.cucudq.cn/gtirlrnjcx.html

按章节统计：
来源：http://hz.gzhubu.top/gtbrpjovdj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhoulong.xyz/gtinbjkjwc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtduqzwpkg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtuksjsojb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xinyue.icu/gtfxwbbkrz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xziqi.cn/gthwyrsyjz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gzhubu.top/gtyyvxvkhy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.havefunace.top/gtsrphnmgk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sysykeji.top/gtrnhjmdab.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtlrgylhxr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.guowangkeji.top/gtykxgvgdi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtwreuahqu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtqtqupbvh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtomlvxdba.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sweek.top/gtojozicgt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.daxiang520.top/gtadenvqwd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtfitdwmcv.html

Q SQL 专题                              90
来源：http://hz.ybcxt.top/gtjjzlivcv.html

R Bash 专题                             80
来源：http://hz.jinqigufen.top/gtjfmxbpth.html

S C / C++ 专题                          60
来源：http://hz.guannengcc.top/gtpkijzqou.html

T 其他语言补充                          60
来源：http://hz.snrcjt.cn/gtthvcfwrf.html

U 高频实用片段                         120
来源：http://hz.xinyue.icu/gtlrzvowez.html

------------------------------------
来源：http://hz.bjfxy.top/gttshpcrso.html

合计                                  2106 条
来源：http://hz.ywan-chungtsiang.top/gtzwykvpke.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtccfuhadm.html

使用提醒
来源：http://hz.cucudq.cn/gtpockwxtt.html

--------------------------------------------------------------------------------
来源：http://hz.ivvv.top/gtiankqevm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinqigfzy.top/gtcffrfpiv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.guannengcc.top/gttidfnxjx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hywenlv.cn/gtacjkieaj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cashguo.top/gtdrvnukeb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cucudq.cn/gtrxltgoza.html

—— 文件结束 ——
来源：http://hz.jinqigfzy.top/gtdjhidyuo.html

================================================================================
来源：http://hz.jianghu66.top/gtnyjmxgjn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nanxinkj.top/gtylowqlyl.html

Common Programming Examples Cheat Book
来源：http://hz.hammf.cn/gtcussyfdr.html

================================================================================
来源：http://hz.tianlin.xyz/gtxxborxpu.html

【收录内容】
来源：http://hz.tanke756.top/gttpyedenb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.bjfxy.top/gtgpwvhlcg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jianghu66.top/gtvkypwqcs.html

SQL · Bash · C · C++
来源：http://hz.pengpengdd.cyou/gtmhdkdkla.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.guowangkeji.top/gtilrfvfud.html

【使用说明】
来源：http://hz.yj20258888.top/gthsoyxeie.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shanyushiyangtech.top/gtwkmszkvn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yvedp.cn/gtfputirci.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xinyue.icu/gtqjeezmve.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.svipenyu.cn/gtvsgcnlas.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hongshengwenyu.top/gtftkzpbjp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.guannengcc.top/gtrpuwepmj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hongshengwenyu.top/gtrgflhmii.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.feifeiyinyue.top/gttpenqeep.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.mhx1999.top/gtsxzbrgxd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhijiandao.cn/gtgoarjxfs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.52xcode.cn/gtzljkbjhi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.guannengcc.top/gtvfybtrkw.html

【文件统计】
来源：http://hz.gogol.net.cn/gtfvrvvjnb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.9152youxi.cn/gtwltbdkhc.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gthsutkshm.html

目  录
来源：http://hz.yonumen.top/gtbpgkersx.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtwmnjxqwy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gtlzjeprvk.html


<!-- 参考信息 -->