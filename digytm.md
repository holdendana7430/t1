代发 wailian999

[U09] Py：字典取最大值的键
来源：http://hz.shuidangran.top/gtyugyokur.html

max(d, key=d.get)
来源：http://hz.9152youxi.cn/gtumwdstta.html

[U10] Py：按值排序字典
来源：http://hz.fengsongda.top/gtwqhufiga.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.kuanghao11.cn/gtarmkloos.html

[U11] Py：生成器表达式
来源：http://hz.xuetiantiany.cn/gtgbleuwxu.html

(x * 2 for x in arr)
来源：http://hz.tian-w.cn/gtnpedtlex.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.meibo888.top/gtceppygsq.html

Counter(arr).most_common(3)
来源：http://hz.aizwys.cn/gtqjrrdgvz.html

[U13] Py：固定长度队列
来源：http://hz.jinqigfzy.top/gthqijtxcx.html

deque(maxlen=10)
来源：http://hz.zhijiandao.cn/gtfcueoimw.html

[U14] Py：分组收集到列表
来源：http://hz.guowangkeji.top/gtwafbtica.html

defaultdict(list)
来源：http://hz.tanke756.top/gtcymrwkmy.html

[U15] Py：高精度计时
来源：http://hz.shangyingyoupin.top/gtbpzjnocw.html

t = time.perf_counter()
来源：http://hz.hongshengwenyu.top/gtafmttqde.html

[U16] Py：命令行参数解析
来源：http://hz.zhaomingkeji.xyz/gtsbxnsmvs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.chenjidiqi.icu/gtwitlrmnd.html

[U17] Py：初始化日志
来源：http://hz.hywenlv.cn/gterkmfnce.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangdashe.top/gtoemmivqk.html

[U18] Py：预编译正则
来源：http://hz.daxiang520.top/gtouiniamr.html

pat = re.compile(r"\d+")
来源：http://hz.meibo888.top/gtvrrnkylc.html

[U19] Py：正则替换带回调
来源：http://hz.hnqzz.top/gtzdwpnqdm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jyoumei.cn/gtawlxvrdj.html

[U20] Py：缓存函数结果
来源：http://hz.chenjidiqi.icu/gttfyxqnne.html

@functools.lru_cache(maxsize=None)
来源：http://hz.guannengcc.top/gttnrozpsb.html

[U21] Py：自定义上下文管理器
来源：http://hz.snrcjt.cn/gteljjfoum.html

@contextlib.contextmanager
来源：http://hz.cdnleiting.top/gtgkwwuntm.html

[U22] Py：矩阵转置
来源：http://hz.jyoumei.cn/gtmpxiyszb.html

list(zip(*m))
来源：http://hz.hammf.cn/gthjlfqkdt.html

[U23] Py：分块读取大文件
来源：http://hz.jinqigfzy.top/gtztyzfkjo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.birdmap.top/gtabbtphqi.html

[U24] Py：路径操作
来源：http://hz.iojbl.cn/gtlzsrhuiu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenjidiqi.icu/gtibekprbe.html

[U25] Py：CSV 按字典读
来源：http://hz.jianghu66.top/gtqehsysrs.html

csv.DictReader(f)
来源：http://hz.cheryme.top/gtuwkicnby.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gttnermcku.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ehwqpu.com/gtamyphbuc.html

[U27] Py：异步 HTTP
来源：http://hz.zhongyouzk.top/gttlegoain.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.pengpengdd.cyou/gtdeydzhgx.html

[U28] Py：类型别名
来源：http://hz.chenjidiqi.icu/gtfmngkfiy.html

UserId = int
来源：http://hz.cdnleiting.top/gtpcdaszjg.html

[U29] Py：属性校验
来源：http://hz.tian-w.cn/gtwalxsgkc.html

@property 与 @x.setter 配合
来源：http://hz.zycfv.cn/gthfrmvcrj.html

[U30] Py：数据类
来源：http://hz.iojbl.cn/gtasoatwmv.html

@dataclass(slots=True)
来源：http://hz.hnqzz.top/gthhwucjcq.html

[U31] Py：单测
来源：http://hz.smart0.xyz/gtqqhnvbri.html

python -m pytest -q
来源：http://hz.gaohongyu789.top/gtumitpowi.html

[U32] Py：代码格式化
来源：http://hz.sxryk.cn/gtqcisjmul.html

ruff format . && ruff check --fix .
来源：http://hz.feifeiyinyue.top/gtyjazugrx.html

[U33] Py：打包发布
来源：http://hz.birdmap.top/gtetvxgxok.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.0kj1m.cn/gtvxsokhfq.html

[U34] Py：判断编码
来源：http://hz.yj202588.top/gtqbzysthd.html

chardet.detect(raw)
来源：http://hz.feifeiyinyue.top/gtdutfnqes.html

[U35] Py：发送邮件
来源：http://hz.cucudq.cn/gtcjruqcsv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.redwolf501.top/gtrxhumrqm.html

[U36] Py：定时任务
来源：http://hz.xuanzx.com/gtplpnptbi.html

schedule.every(10).minutes.do(job)
来源：http://hz.jyoumei.cn/gtyksjvjao.html

[U37] Py：读写 Excel
来源：http://hz.gaohongyu789.top/gtvzimtvwf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zycfv.cn/gtkwxggyfc.html

[U38] Py：获取脚本所在目录
来源：http://hz.yj20258.top/gtcyvnhyhb.html

Path(__file__).resolve().parent
来源：http://hz.vqdsnc.cn/gtapfpiuqb.html

[U39] Py：判断是否在交互环境
来源：http://hz.xinyue.icu/gtxtuwjrra.html

sys.stdout.isatty()
来源：http://hz.sweek.top/gtvbxaknir.html

[U40] Py：打印到标准错误
来源：http://hz.guowangkeji.top/gtnxihrzmk.html

print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtwvzwhnpg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.feifeiyinyue.top/gteyhctmdw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.dashuyun.cn/gtqypzehzb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhaomingkeji.xyz/gtxusvcqkr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.iojbl.cn/gthptnotxy.html

[U43] PHP：声明命名空间
来源：http://hz.xinyue.icu/gtbtkxwdpf.html

namespace App\Http;
来源：http://hz.fengsongda.top/gtdzthzbel.html

[U44] PHP：开启严格类型
来源：http://hz.sufxvd.cn/gtwocecjbg.html

declare(strict_types=1);
来源：http://hz.52xcode.cn/gtmrqimgzg.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sufxvd.cn/gtvjbrlsbs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtpaclqyxv.html

[U46] PHP：可空类型
来源：http://hz.jinghuilouyu.cn/gtpqleuesx.html

?string $name = null
来源：http://hz.shanyushiyangtech.top/gtcftwkvdt.html

[U47] PHP：联合类型
来源：http://hz.guowangkeji.top/gtbezqytlg.html

int|string $id
来源：http://hz.jinyuanbaomall.cn/gtnetcjhtk.html

[U48] PHP：纯枚举
来源：http://hz.ybcxt.top/gtnozpupsh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.guowangkeji.top/gtpnosubvk.html

[U49] PHP：只读属性
来源：http://hz.haohaochexian.top/gtihzvqxzl.html

public readonly string $name
来源：http://hz.xuetiantiany.cn/gtrjddmgow.html

[U50] PHP：构造器属性提升
来源：http://hz.ppjwa.cn/gttumytguk.html

public function __construct(private int $id) {}
来源：http://hz.ppjwa.cn/gtyvsteqbi.html

[U51] PHP：数组解构
来源：http://hz.nanxuanxn.top/gtqsiggpyj.html

[$a, $b] = $arr;
来源：http://hz.zhoulong.xyz/gtfzyxrmik.html

[U52] PHP：箭头函数
来源：http://hz.yanxiufei.cn/gtxzsxoves.html

$double = fn($x) => $x * 2;
来源：http://hz.kuanghao11.cn/gtxrkbzemv.html

[U53] PHP：空合并运算符
来源：http://hz.dashuyun.cn/gtdfbwumww.html

$v = $a ?? $b ?? "default";
来源：http://hz.quarkkingdee.top/gtkmixyrjf.html

[U54] PHP：空安全调用
来源：http://hz.jyoumei.cn/gtlfshrjqf.html

$obj?->method()
来源：http://hz.daxiang520.top/gttqeqjbeh.html

[U55] PHP：match 表达式
来源：http://hz.pycfn.com/gttfyoeoqi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.chenjidiqi.icu/gtdqunxgpe.html

[U56] PHP：命名参数
来源：http://hz.ydzc1.top/gtvajsrelx.html

f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gtfhztrgie.html

[U57] PHP：字符串插值
来源：http://hz.ydjk.org.cn/gtokvzpdby.html

"值: {$a}"
来源：http://hz.tian-w.cn/gtphvghesw.html

[U58] PHP：数组三件套
来源：http://hz.daxiang520.top/gtzmeametd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yangfankeji.com/gtyedanwtt.html

[U59] PHP：自定义排序
来源：http://hz.zhongyouzk.top/gttdttmvhu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtownqrbxm.html

[U60] PHP：JSON 编解码
来源：http://hz.hnxiangtu.top/gttqsmzpwu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guowangkeji.top/gtrztipapm.html

[U61] PHP：正则
来源：http://hz.tian-w.cn/gtrtaphtvh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtjkwuvnag.html

[U62] PHP：日期对象
来源：http://hz.andypj.xyz/gtfmnmitoj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.haohaochexian.top/gtetnrxeda.html

[U63] PHP：文件读写
来源：http://hz.wangdashe.top/gtaeqfesfq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhaomingkeji.xyz/gtbpryronk.html

[U64] PHP：目录遍历
来源：http://hz.gotoacloud.top/gtvnzykree.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj20258888.top/gthyfpubbx.html

[U65] PHP：会话
来源：http://hz.sxryk.cn/gtxtibpwhh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gogol.net.cn/gtyyslcrwv.html

[U66] PHP：设置 Cookie
来源：http://hz.ywan-chungtsiang.top/gtvtlkstmg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinqigufen.top/gteabmzzpf.html

[U67] PHP：处理文件上传
来源：http://hz.chenlongwang.top/gtjqembpxd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.316326.xyz/gtaavgsfni.html

[U68] PHP：PDO 连接
来源：http://hz.hnxiangtu.top/gtkuntgmgd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhongyouzk.top/gttcyiubut.html

[U69] PHP：PDO 预处理
来源：http://hz.bjfxy.top/gtikufdrva.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhaomingkeji.xyz/gtchstsxzs.html

[U70] PHP：PDO 事务
来源：http://hz.jyoumei.cn/gtxajuwxxr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.guowangkeji.top/gtybhdnbvt.html

[U71] PHP：抛出异常
来源：http://hz.cashguo.top/gtelyxhgan.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhongyouzk.top/gtvywcoxiq.html

[U72] PHP：写错误日志
来源：http://hz.hnxiangtu.top/gtrnmjgzps.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cashguo.top/gtbmvvjnwh.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenjidiqi.icu/gtmrblvdcn.html

parse_ini_file("config.ini", true)
来源：http://hz.yongpay.top/gtvgfjpwnp.html

[U74] PHP：读取环境变量
来源：http://hz.svipenyu.cn/gtpnfugtfd.html

getenv("APP_ENV") ?: "production"
来源：http://hz.9152youxi.cn/gtinmphzcm.html

[U75] PHP：依赖注入
来源：http://hz.ivvv.top/gtcihjnvuj.html

composer require psr/container
来源：http://hz.tianlin.xyz/gtyjyezdgg.html

[U76] PHP：简单路由
来源：http://hz.nanxinkj.top/gtkvcknvmc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shzxlz.cn/gtnlduhtmo.html

[U77] PHP：模板渲染
来源：http://hz.xylfe.cn/gtrzdxnxll.html

composer require twig/twig
来源：http://hz.ywan-chungtsiang.top/gtuwwlmjtm.html

[U78] PHP：单元测试
来源：http://hz.tian-w.cn/gtzbmdvwat.html

composer require --dev phpunit/phpunit
来源：http://hz.yanxiufei.cn/gtfqgjaphq.html

[U79] PHP：静态分析
来源：http://hz.tanke756.top/gtwzzyttfr.html

composer require --dev phpstan/phpstan
来源：http://hz.tanke756.top/gtuaopyooq.html

[U80] PHP：代码规范修复
来源：http://hz.cdnleiting.top/gttxmeywdv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yuanzhike.top/gtrvzxonmo.html

[U81] JS：初始化项目
来源：http://hz.zhiwuduotai.top/gtmrogxpsd.html

npm init -y;  npm i express
来源：http://hz.zhiwuduotai.top/gtjzwihcnc.html

[U82] JS：package.json 脚本
来源：http://hz.tanke756.top/gthcxsavvw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ybcxt.top/gtkghdfnut.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhijiandao.cn/gtfmujyher.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xingfuxueyuan.xyz/gtbnytvwfs.html

[U84] JS：CommonJS 写法
来源：http://hz.zhaomingkeji.xyz/gtkhoarwvc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.meibo888.top/gtcbfydxro.html

[U85] JS：可选链
来源：http://hz.redwolf501.top/gtxzvlqcnj.html

a?.b?.c
来源：http://hz.xuetiantiany.cn/gtndkpydvo.html

[U86] JS：空值合并
来源：http://hz.yj20258888.top/gttqfzsfik.html

a ?? b
来源：http://hz.shuidangran.top/gtjppsejer.html

[U87] JS：解构默认值
来源：http://hz.andypj.xyz/gthnolbymc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cdnleiting.top/gtnabchhzb.html

[U88] JS：对象展开合并
来源：http://hz.ydjk.org.cn/gtfmspthia.html

{ ...a, ...b }
来源：http://hz.gogol.net.cn/gtabztbsfg.html

[U89] JS：数组去重
来源：http://hz.xziqi.cn/gtmvnrgmmg.html

[...new Set(arr)]
来源：http://hz.jianghu66.top/gtzhsnzfza.html

[U90] JS：数字数组排序
来源：http://hz.kuanghao11.cn/gtqblfcabh.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtgtlfnioa.html

[U91] JS：对象键值遍历
来源：http://hz.zhongyouzk.top/gtkedbrboz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jqgfzy.top/gtgmggzgst.html

[U92] JS：深拷贝
来源：http://hz.jiagoushi.top/gtjhozgklb.html

structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtimnivdnz.html

[U93] JS：模板字符串
来源：http://hz.zhoulong.xyz/gtjbbvnigk.html

`共 ${n} 条`
来源：http://hz.xuanzx.com/gtcgtnhche.html

[U94] JS：箭头函数
来源：http://hz.yonumen.top/gtwfsvhoqx.html

const double = x => x * 2;
来源：http://hz.kuanghao11.cn/gtfuiuybcl.html

[U95] JS：Promise 包装
来源：http://hz.yvedp.cn/gtcdaicspf.html

new Promise((resolve, reject) => {})
来源：http://hz.jianghu66.top/gtydufaltd.html

[U96] JS：async/await 与异常
来源：http://hz.hnqzz.top/gtnjngxigq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigufen.top/gtslnyjjue.html

[U97] JS：并发请求
来源：http://hz.chenjidiqi.icu/gtemhesfyw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtekczbwbt.html

[U98] JS：fetch 带 JSON
来源：http://hz.hfpthk.cn/gtiuoknbpr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pycfn.com/gtinmvgfhp.html

[U99] JS：事件监听
来源：http://hz.cheryme.top/gtnzqdoqfl.html

el.addEventListener("click", e => {})
来源：http://hz.cqqwz.cn/gtgyiidzre.html

[U100] JS：DOM 查询
来源：http://hz.9152youxi.cn/gtezkfmqlg.html

document.querySelector(".item")
来源：http://hz.jqgfzy.top/gtzlwzpkqs.html

[U101] JS：classList 操作
来源：http://hz.52xcode.cn/gtgsyqmcbq.html

el.classList.toggle("active")
来源：http://hz.kuanghao11.cn/gtndrloqcc.html

[U102] JS：本地存储
来源：http://hz.smart0.xyz/gtbqzpjhby.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuanzhike.top/gtvznlearb.html

[U103] JS：定时器
来源：http://hz.cqqwz.cn/gtbnrjebco.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ppjwa.cn/gttohhplyy.html

[U104] JS：防抖
来源：http://hz.kuanghao11.cn/gtesmvkops.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtpzuijlso.html

[U105] JS：节流
来源：http://hz.bjfxy.top/gttdstldcr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.andypj.xyz/gtwwlmerct.html

[U106] JS：日期格式化
来源：http://hz.redwolf501.top/gtsgnxfspg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ivvv.top/gtzblolhdm.html

[U107] JS：数字千分位
来源：http://hz.316326.xyz/gtqxirtvpd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ivvv.top/gtfclxqtxu.html

[U108] JS：随机整数
来源：http://hz.yj202588.top/gtuduzmmcn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tanke756.top/gtwccfuqnb.html

[U109] JS：数组分组
来源：http://hz.sxryk.cn/gtrfcsjuqf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ppjwa.cn/gtbdbuamzb.html

[U110] JS：数组分块
来源：http://hz.jqgfzy.top/gtmkoydmaa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hnxiangtu.top/gtfwdhjuiz.html

[U111] JS：对象转 Map
来源：http://hz.jiagoushi.top/gtfsianwcy.html

new Map(Object.entries(obj))
来源：http://hz.iojbl.cn/gtwslrksgp.html

[U112] JS：字符串补位
来源：http://hz.yanxiufei.cn/gtczowhipj.html

"7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtqufmdfva.html

[U113] JS：正则替换全部
来源：http://hz.zhixingplan.top/gtjgqlgbmv.html

s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtycxnvugi.html

[U114] JS：JSON 深比较
来源：http://hz.pengpengdd.cyou/gtxjlfkvnr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtmxmzfpel.html

[U115] JS：生成 UUID
来源：http://hz.nanxuanxn.top/gtludwwfyx.html

crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtqynujzjd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shanyushiyangtech.top/gttekebjrf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.meibo888.top/gtyrlmigll.html

[U117] JS：单元测试
来源：http://hz.cucudq.cn/gtppycrazt.html

npm i -D vitest;  npx vitest
来源：http://hz.xylfe.cn/gtanekzuqw.html

[U118] JS：开发服务器
来源：http://hz.xylfe.cn/gthmaqyoos.html

npm i -D vite;  npx vite
来源：http://hz.daria6918.cn/gtgrhhprew.html

[U119] JS：生产构建
来源：http://hz.daxiang520.top/gtenptebee.html

npx vite build
来源：http://hz.smart0.xyz/gterylgxyz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sxryk.cn/gtwzztydjp.html

import.meta.env.VITE_API_URL
来源：http://hz.zhengqikj.top/gtzowvxtai.html

================================================================================
来源：http://hz.0kj1m.cn/gtbykcaajf.html

统计汇总
来源：http://hz.316326.xyz/gtezyrwemh.html

================================================================================
来源：http://hz.iojbl.cn/gtldhbfhbp.html

按语言统计（条）：
来源：http://hz.xylfe.cn/gteygbaacz.html

Python ......... 252
来源：http://hz.yvedp.cn/gtmjjrtomn.html

PHP ............ 252
来源：http://hz.yuxming.cn/gtqyiimmgn.html

JavaScript ..... 252
来源：http://hz.guannengcc.top/gtwrknsszk.html

TypeScript ..... 212
来源：http://hz.ydjk.org.cn/gtyjzjezcz.html

Java ........... 212
来源：http://hz.zhixingplan.top/gtmnmlctgn.html

Go ............. 212
来源：http://hz.sxryk.cn/gtzsrztgze.html

Ruby ........... 212
来源：http://hz.sxryk.cn/gtbvkaaqqy.html

C# ............. 212
来源：http://hz.jiagoushi.top/gttasjcwtq.html

C .............. 30
来源：http://hz.hnqzz.top/gthxcswrrk.html

C++ ............ 30
来源：http://hz.ydjk.org.cn/gtzvualzcj.html

SQL ............ 90
来源：http://hz.hammf.cn/gtctzvmnsr.html

Bash ........... 80
来源：http://hz.jinqigufen.top/gtepioqcjs.html

Kotlin ......... 15
来源：http://hz.zhoulong.xyz/gtgnapkvza.html

Swift .......... 15
来源：http://hz.hnxiangtu.top/gtsjkvyqlk.html

Lua ............ 10
来源：http://hz.jyoumei.cn/gtvyhoqbme.html

Perl ........... 10
来源：http://hz.andypj.xyz/gtzucabbac.html

Scala .......... 10
来源：http://hz.yuxming.cn/gtdttejlhx.html

------------------------------------
来源：http://hz.zhengqikj.top/gthbzvkcii.html

合计 ........... 2106 条
来源：http://hz.shuidangran.top/gtfszzklpd.html

按章节统计：
来源：http://hz.yongpay.top/gtzivexktn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jiagoushi.top/gteqxahvfa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtpdhzwzbq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.havefunace.top/gtoxctghve.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtakxjjety.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.feifeiyinyue.top/gtcxrkqrvd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sweek.top/gtyppwbeeg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gtmtpohoer.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.9152youxi.cn/gtycfqwgwx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtmolukedt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtdwqxdxam.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtzfnzcceb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtqnrhuhyp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtxdkdcofk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtaexqcjfl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xziqi.cn/gtbxcamhgd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtklwwnand.html

Q SQL 专题                              90
来源：http://hz.shanyushiyangkeji.top/gtffvquiih.html

R Bash 专题                             80
来源：http://hz.jqgufenzy.top/gtmjnjhmdx.html

S C / C++ 专题                          60
来源：http://hz.ydjk.org.cn/gtcwfoxflg.html

T 其他语言补充                          60
来源：http://hz.guowangkeji.top/gtmxxprghm.html

U 高频实用片段                         120
来源：http://hz.ywan-chungtsiang.top/gtkkicykjy.html

------------------------------------
来源：http://hz.shzxlz.cn/gthrzaocgz.html

合计                                  2106 条
来源：http://hz.gaohongyu789.top/gtutgwhkon.html

--------------------------------------------------------------------------------
来源：http://hz.aibaodan.cn/gtmbvobfye.html

使用提醒
来源：http://hz.yj20258888.top/gtyawcwupp.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtyiqcxobf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nwbrower.top/gtwxylryfv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.fengsongda.top/gtxrcjwnwi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhijiandao.cn/gtrpigitkt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hnxiangtu.top/gtgxyezkuu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xziqi.cn/gtrkpocuzv.html

—— 文件结束 ——
来源：http://hz.shuidangran.top/gtzkycxqeg.html

================================================================================
来源：http://hz.316326.xyz/gtonqyhgbh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xziqi.cn/gtpitdmvns.html

Common Programming Examples Cheat Book
来源：http://hz.jqgfzy.top/gtwmklrwfq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyqlhzdof.html

【收录内容】
来源：http://hz.pycfn.com/gtstssmrgs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.nanxuanxn.top/gtfmxvdwzg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhixingplan.top/gteorpngbe.html

SQL · Bash · C · C++
来源：http://hz.mhx1999.top/gtikxwmmkg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hnxiangtu.top/gtylyfadvj.html

【使用说明】
来源：http://hz.shuidangran.top/gtfnmeatis.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.guowangkeji.top/gtjjgdglmd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daxiang520.top/gtwpnavmnw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jiagoushi.top/gtfkjzvdvj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yongpay.top/gtpakauwyo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ydjk.org.cn/gtihulutdm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gogol.net.cn/gtrptgmejd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.cheryme.top/gtjkqincsd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ppjwa.cn/gtpqyfnmer.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cucudq.cn/gtvqgappbs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhoulong.xyz/gttpmiqpge.html


<!-- 参考信息 -->