代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhoulong.xyz/gtjnqrrkon.html

[T59] Scala：循环
来源：http://hz.bjfxy.top/gtgbqsluum.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuanzx.com/gtzcgnszph.html

[T60] Scala：折叠
来源：http://hz.dianchejie.cn/gtccmmuznt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinqigfzy.top/gtmmdfwafs.html

================================================================================
来源：http://hz.xylfe.cn/gtgrraeexu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cucudq.cn/gtcynbbxio.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcvjicovg.html

[U01] Py：创建虚拟环境
来源：http://hz.ehwqpu.com/gtgpauhaol.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tanke756.top/gtdnkivqpw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.snrcjt.cn/gtpcyrepqz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dianchejie.cn/gtjwtmjsji.html

[U03] Py：加载 .env 配置
来源：http://hz.mhx1999.top/gtacikhtcn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenjidiqi.icu/gtkzcodxpl.html

[U04] Py：变量调试打印
来源：http://hz.yj20258.top/gtrggrpwhr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sufxvd.cn/gtsyqbrzbk.html

[U05] Py：列表去重且保序
来源：http://hz.zhaomingkeji.xyz/gtkiskdaug.html

list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtscrwheii.html

[U06] Py：合并两个字典
来源：http://hz.shangyingyoupin.top/gtjjkywqhb.html

{**a, **b}
来源：http://hz.shanyushiyangtech.top/gtarcqdarq.html

[U07] Py：反转字典键值
来源：http://hz.ivvv.top/gtshqkckyj.html

{v: k for k, v in d.items()}
来源：http://hz.jiagoushi.top/gtzvbtxugr.html

[U08] Py：展平二维列表
来源：http://hz.xylfe.cn/gtahinhnhu.html

[y for x in nested for y in x]
来源：http://hz.wangdashe.top/gtggwdrycm.html

[U09] Py：字典取最大值的键
来源：http://hz.kuanghao11.cn/gtpgsfmmaj.html

max(d, key=d.get)
来源：http://hz.pycfn.com/gtxmdxdfwd.html

[U10] Py：按值排序字典
来源：http://hz.hnxiangtu.top/gtumywzevo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnqzz.top/gtyrzfscyo.html

[U11] Py：生成器表达式
来源：http://hz.vqdsnc.cn/gtfdzwyhar.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gttcawfnph.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gzhubu.top/gtyiyqsnsm.html

Counter(arr).most_common(3)
来源：http://hz.yj20258888.top/gtyoqqmwcl.html

[U13] Py：固定长度队列
来源：http://hz.xylfe.cn/gtzvsnouar.html

deque(maxlen=10)
来源：http://hz.jyoumei.cn/gtthcfaqdl.html

[U14] Py：分组收集到列表
来源：http://hz.guannengcc.top/gtmvykekwe.html

defaultdict(list)
来源：http://hz.cqqwz.cn/gtrzkycjgk.html

[U15] Py：高精度计时
来源：http://hz.zhongyouzk.top/gtvjjdnnzv.html

t = time.perf_counter()
来源：http://hz.havefunace.top/gtzxboyten.html

[U16] Py：命令行参数解析
来源：http://hz.shangyingyoupin.top/gtunezzsmx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhoulong.xyz/gtcqbborba.html

[U17] Py：初始化日志
来源：http://hz.tian-w.cn/gtufjqbqag.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhongyouzk.top/gtofxofhva.html

[U18] Py：预编译正则
来源：http://hz.quarkkingdee.top/gtsgwzepnv.html

pat = re.compile(r"\d+")
来源：http://hz.xziqi.cn/gtyyrynncm.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigufen.top/gtafcimhvw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinqigfzy.top/gtoqdxdull.html

[U20] Py：缓存函数结果
来源：http://hz.zhoulong.xyz/gtgwgfqzjm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cqqwz.cn/gtnrqwoecm.html

[U21] Py：自定义上下文管理器
来源：http://hz.ppjwa.cn/gtrdbknryv.html

@contextlib.contextmanager
来源：http://hz.daxiang520.top/gtdyghrlhi.html

[U22] Py：矩阵转置
来源：http://hz.52xcode.cn/gtqhiaepbz.html

list(zip(*m))
来源：http://hz.cdnleiting.top/gtkipexpsc.html

[U23] Py：分块读取大文件
来源：http://hz.c1oappe.top/gtcbctwahj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shzxlz.cn/gtlopfefqu.html

[U24] Py：路径操作
来源：http://hz.zhengqikj.top/gtzveyrswg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.vqdsnc.cn/gtxkmzthej.html

[U25] Py：CSV 按字典读
来源：http://hz.wangdashe.top/gtarblfptx.html

csv.DictReader(f)
来源：http://hz.xinyue.icu/gtmaggdqfx.html

[U26] Py：并发下载
来源：http://hz.nanxinkj.top/gtaezhewhp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.bjfxy.top/gtxunxprkf.html

[U27] Py：异步 HTTP
来源：http://hz.aizwys.cn/gtczsgsmwg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.iojbl.cn/gtacsdkyay.html

[U28] Py：类型别名
来源：http://hz.yuxming.cn/gttsyzajlb.html

UserId = int
来源：http://hz.hnqzz.top/gtcskwukmt.html

[U29] Py：属性校验
来源：http://hz.tian-w.cn/gthroqretq.html

@property 与 @x.setter 配合
来源：http://hz.xuetiantiany.cn/gtqsstlarn.html

[U30] Py：数据类
来源：http://hz.hysaishi.cn/gtpjeucspc.html

@dataclass(slots=True)
来源：http://hz.316326.xyz/gttoxawujy.html

[U31] Py：单测
来源：http://hz.quarkkingdee.top/gtqkscdssr.html

python -m pytest -q
来源：http://hz.yj20258888.top/gtzwykmneh.html

[U32] Py：代码格式化
来源：http://hz.ppjwa.cn/gthtmzwfdg.html

ruff format . && ruff check --fix .
来源：http://hz.dianchejie.cn/gttnfwxriw.html

[U33] Py：打包发布
来源：http://hz.cdnleiting.top/gtlwkkjkyi.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.tanke756.top/gtergwznld.html

[U34] Py：判断编码
来源：http://hz.jianghu66.top/gtsbodstmu.html

chardet.detect(raw)
来源：http://hz.guowangkeji.top/gtbzzvbpxu.html

[U35] Py：发送邮件
来源：http://hz.zhixingplan.top/gtmvleyiqg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xinyue.icu/gtgkyqtcyj.html

[U36] Py：定时任务
来源：http://hz.tian-w.cn/gtexdmcdor.html

schedule.every(10).minutes.do(job)
来源：http://hz.ydjk.org.cn/gtvhmrqien.html

[U37] Py：读写 Excel
来源：http://hz.xuetiantiany.cn/gtuyikhopc.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.gzhubu.top/gtlukeujvd.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhixingplan.top/gtaszsipvr.html

Path(__file__).resolve().parent
来源：http://hz.mhx1999.top/gtqfguawit.html

[U39] Py：判断是否在交互环境
来源：http://hz.havefunace.top/gtssykrzcn.html

sys.stdout.isatty()
来源：http://hz.wangshuangyany.cn/gtaxiflkty.html

[U40] Py：打印到标准错误
来源：http://hz.cashguo.top/gtkswjsaqc.html

print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtfsfzbcrx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.aibaodan.cn/gthqknpzcm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tianlin.xyz/gtgfslosji.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.meibo888.top/gtduulbtvi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cucudq.cn/gtysujirri.html

[U43] PHP：声明命名空间
来源：http://hz.ivvv.top/gtdetsmptn.html

namespace App\Http;
来源：http://hz.ybcxt.top/gtblwyensv.html

[U44] PHP：开启严格类型
来源：http://hz.gzhubu.top/gtvxgbkvib.html

declare(strict_types=1);
来源：http://hz.gaohongyu789.top/gtxhftadkf.html

[U45] PHP：类型声明与返回类型
来源：http://hz.aibaodan.cn/gtljpmahre.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yanxiufei.cn/gtjjltxwvi.html

[U46] PHP：可空类型
来源：http://hz.ivvv.top/gtlgpevnee.html

?string $name = null
来源：http://hz.vqdsnc.cn/gtokyudsuz.html

[U47] PHP：联合类型
来源：http://hz.guannengcc.top/gtuyrdlwya.html

int|string $id
来源：http://hz.iojbl.cn/gtwnpdylsc.html

[U48] PHP：纯枚举
来源：http://hz.nwbrower.top/gtzfcpoebw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.dashuyun.cn/gtpefuemju.html

[U49] PHP：只读属性
来源：http://hz.daxiang520.top/gtdxzraoml.html

public readonly string $name
来源：http://hz.quarkkingdee.top/gtmznudowh.html

[U50] PHP：构造器属性提升
来源：http://hz.hnqzz.top/gtchscjoig.html

public function __construct(private int $id) {}
来源：http://hz.yueranfly.top/gtvglzptzd.html

[U51] PHP：数组解构
来源：http://hz.jqgfzy.top/gtfzcwzynl.html

[$a, $b] = $arr;
来源：http://hz.xziqi.cn/gtrnokfcgs.html

[U52] PHP：箭头函数
来源：http://hz.yueranfly.top/gteedvhtbf.html

$double = fn($x) => $x * 2;
来源：http://hz.chenlongwang.top/gtaxvgwpjf.html

[U53] PHP：空合并运算符
来源：http://hz.andypj.xyz/gtopvqsxdr.html

$v = $a ?? $b ?? "default";
来源：http://hz.ehwqpu.com/gtwcqgmusq.html

[U54] PHP：空安全调用
来源：http://hz.jyoumei.cn/gtcnnqedwq.html

$obj?->method()
来源：http://hz.xinyue.icu/gtjkponttl.html

[U55] PHP：match 表达式
来源：http://hz.cashguo.top/gtnmswxcha.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.316326.xyz/gtxoxoetgj.html

[U56] PHP：命名参数
来源：http://hz.dashuyun.cn/gtpwxpgnvw.html

f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtepavslkf.html

[U57] PHP：字符串插值
来源：http://hz.ybcxt.top/gturlaanrb.html

"值: {$a}"
来源：http://hz.jyoumei.cn/gtnyxzyrnn.html

[U58] PHP：数组三件套
来源：http://hz.quarkkingdee.top/gtwvfumhge.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yvedp.cn/gttwreeuhk.html

[U59] PHP：自定义排序
来源：http://hz.xuanzx.com/gtzgqinhuq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xziqi.cn/gtkoldkjdg.html

[U60] PHP：JSON 编解码
来源：http://hz.nwbrower.top/gtunagtcfp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yueranfly.top/gtpbcgqmoz.html

[U61] PHP：正则
来源：http://hz.aibaodan.cn/gtiqvqgojr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shzxlz.cn/gtdqzbdumi.html

[U62] PHP：日期对象
来源：http://hz.sweek.top/gteoysvphk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cashguo.top/gtxctxjdxf.html

[U63] PHP：文件读写
来源：http://hz.jianghu66.top/gtychklgqs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xinyue.icu/gtedsemrju.html

[U64] PHP：目录遍历
来源：http://hz.haohaochexian.top/gtlgvocrsf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.birdmap.top/gtmhyhgtps.html

[U65] PHP：会话
来源：http://hz.fzhhl.top/gtfdflreuo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangdashe.top/gtiyliqbmd.html

[U66] PHP：设置 Cookie
来源：http://hz.shanyushiyangtech.top/gtxfcxmbgs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.smart0.xyz/gtqdzcfnqc.html

[U67] PHP：处理文件上传
来源：http://hz.dianchejie.cn/gtyiniddvn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shuidangran.top/gttufzngxs.html

[U68] PHP：PDO 连接
来源：http://hz.havefunace.top/gtvzrrixkd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.haohaochexian.top/gtjglktlwq.html

[U69] PHP：PDO 预处理
来源：http://hz.ydzc1.top/gtokjiwddo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinghuilouyu.cn/gtgiycqpcb.html

[U70] PHP：PDO 事务
来源：http://hz.52xcode.cn/gtowtmezvh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hnxiangtu.top/gtcbtaigjb.html

[U71] PHP：抛出异常
来源：http://hz.snrcjt.cn/gtmflzvmll.html

throw new RuntimeException("失败", 500);
来源：http://hz.chenzaomai.com/gtoikuvjov.html

[U72] PHP：写错误日志
来源：http://hz.xylfe.cn/gtfxccggcp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhixingplan.top/gtchuinlfp.html

[U73] PHP：读取 ini 配置
来源：http://hz.cqqwz.cn/gtgtlblrnt.html

parse_ini_file("config.ini", true)
来源：http://hz.nanxuanxn.top/gtauqsrlln.html

[U74] PHP：读取环境变量
来源：http://hz.zdqjudy.top/gtfdiypptj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yuxming.cn/gtgflxcpsg.html

[U75] PHP：依赖注入
来源：http://hz.xuetiantiany.cn/gtykpptwgu.html

composer require psr/container
来源：http://hz.wangdashe.top/gtzqlcemuu.html

[U76] PHP：简单路由
来源：http://hz.xinyue.icu/gtfvhaouqr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.meibo888.top/gtkcmnrbmo.html

[U77] PHP：模板渲染
来源：http://hz.gaohongyu789.top/gtnfxtkagi.html

composer require twig/twig
来源：http://hz.mhx1999.top/gtnzlrjsla.html

[U78] PHP：单元测试
来源：http://hz.bjfxy.top/gtwfozbgxw.html

composer require --dev phpunit/phpunit
来源：http://hz.xuanzx.com/gtmzucxlea.html

[U79] PHP：静态分析
来源：http://hz.xingfuxueyuan.xyz/gtkvgxttkw.html

composer require --dev phpstan/phpstan
来源：http://hz.cucudq.cn/gtsvqmgizo.html

[U80] PHP：代码规范修复
来源：http://hz.shanyushiyangkeji.top/gtteekifzo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhengqikj.top/gtzqahgarq.html

[U81] JS：初始化项目
来源：http://hz.meibo888.top/gtbkquemlp.html

npm init -y;  npm i express
来源：http://hz.xziqi.cn/gtakrbmkbm.html

[U82] JS：package.json 脚本
来源：http://hz.zycfv.cn/gtuxeznddo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cqqwz.cn/gtpfspnaml.html

[U83] JS：ES Module 导入导出
来源：http://hz.chenjidiqi.icu/gtdgnbzdmw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cheryme.top/gtjppdtxuj.html

[U84] JS：CommonJS 写法
来源：http://hz.zhoulong.xyz/gticdxjooz.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yonumen.top/gtoolyesjz.html

[U85] JS：可选链
来源：http://hz.haohaochexian.top/gtjvmpbtzr.html

a?.b?.c
来源：http://hz.haohaochexian.top/gtgxumjlrf.html

[U86] JS：空值合并
来源：http://hz.316326.xyz/gtpanrwzhn.html

a ?? b
来源：http://hz.ppjwa.cn/gtviekeeju.html

[U87] JS：解构默认值
来源：http://hz.zdqjudy.top/gtrvzepipt.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinyuanbaomall.cn/gtffalgspv.html

[U88] JS：对象展开合并
来源：http://hz.316326.xyz/gtokayoebb.html

{ ...a, ...b }
来源：http://hz.smart0.xyz/gtgertabmi.html

[U89] JS：数组去重
来源：http://hz.cucudq.cn/gthazfqxmm.html

[...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtzileynwv.html

[U90] JS：数字数组排序
来源：http://hz.316326.xyz/gtyvinehvw.html

[...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtccuiehcj.html

[U91] JS：对象键值遍历
来源：http://hz.aibaodan.cn/gtsulbjtat.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.tian-w.cn/gtoygkssnb.html

[U92] JS：深拷贝
来源：http://hz.cdnleiting.top/gtinajjdgv.html

structuredClone(obj)
来源：http://hz.iojbl.cn/gtzwijcnfs.html

[U93] JS：模板字符串
来源：http://hz.ehwqpu.com/gtdrtdugcr.html

`共 ${n} 条`
来源：http://hz.hnqzz.top/gttbiemfez.html

[U94] JS：箭头函数
来源：http://hz.wangdashe.top/gtabvzixhc.html

const double = x => x * 2;
来源：http://hz.iojbl.cn/gtlzlefbew.html

[U95] JS：Promise 包装
来源：http://hz.jyoumei.cn/gtdmikvzih.html

new Promise((resolve, reject) => {})
来源：http://hz.jinqigufen.top/gtfbpwfzpz.html

[U96] JS：async/await 与异常
来源：http://hz.chenjidiqi.icu/gtzmqldcku.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yonumen.top/gtnzqsswul.html

[U97] JS：并发请求
来源：http://hz.dashuyun.cn/gthwegzkka.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtfuaoqfeb.html

[U98] JS：fetch 带 JSON
来源：http://hz.yvedp.cn/gttngzxevc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhongyouzk.top/gteityxaun.html

[U99] JS：事件监听
来源：http://hz.ydzc1.top/gtgseyxxfq.html

el.addEventListener("click", e => {})
来源：http://hz.jyoumei.cn/gtojmynfqa.html

[U100] JS：DOM 查询
来源：http://hz.svipenyu.cn/gtwmnhsnyk.html

document.querySelector(".item")
来源：http://hz.snrcjt.cn/gtldkyiuzl.html

[U101] JS：classList 操作
来源：http://hz.xingfuxueyuan.xyz/gtjyhtotse.html

el.classList.toggle("active")
来源：http://hz.aizwys.cn/gtqqsszian.html

[U102] JS：本地存储
来源：http://hz.52xcode.cn/gtrthluqlx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jlsjyb.cn/gtmhklusak.html

[U103] JS：定时器
来源：http://hz.shzxlz.cn/gtpstbsery.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.bjfxy.top/gtkbijgzhh.html

[U104] JS：防抖
来源：http://hz.hnqzz.top/gtblvxkxnr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtmbsgyrrj.html

[U105] JS：节流
来源：http://hz.shangyingyoupin.top/gtudbdqufm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.sxryk.cn/gtyyokvehr.html

[U106] JS：日期格式化
来源：http://hz.hongshengwenyu.top/gtexhfbpkf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.meibo888.top/gtuamlhbjp.html

[U107] JS：数字千分位
来源：http://hz.andypj.xyz/gtkqzuwnbu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ydzc1.top/gtylpbjxvy.html

[U108] JS：随机整数
来源：http://hz.yj202588.top/gtxhjjvjlw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guowangkeji.top/gtqzudtyxh.html

[U109] JS：数组分组
来源：http://hz.52xcode.cn/gtfsfuokao.html

Object.groupBy(arr, x => x.type)
来源：http://hz.chenlongwang.top/gtupjjyfzb.html

[U110] JS：数组分块
来源：http://hz.jyoumei.cn/gtovjqoigt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinghuilouyu.cn/gtrbvwuoko.html

[U111] JS：对象转 Map
来源：http://hz.cheryme.top/gtcumbteur.html

new Map(Object.entries(obj))
来源：http://hz.bjfxy.top/gtgogfvhhs.html

[U112] JS：字符串补位
来源：http://hz.yongpay.top/gtfozfuarg.html

"7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gtxrwgvyqe.html

[U113] JS：正则替换全部
来源：http://hz.iojbl.cn/gtucsrscrs.html

s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtazuhyymt.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigufen.top/gtjpjkswlw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtuvemgbqy.html

[U115] JS：生成 UUID
来源：http://hz.jianghu66.top/gtfqcqqzzq.html

crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtbhgoouql.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhixingplan.top/gtgskwtuke.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yvedp.cn/gtfwiaqelm.html

[U117] JS：单元测试
来源：http://hz.jiagoushi.top/gtiscpkbpn.html

npm i -D vitest;  npx vitest
来源：http://hz.jinyuanbaomall.cn/gtpusjtuey.html

[U118] JS：开发服务器
来源：http://hz.yanxiufei.cn/gtbcpfjclh.html

npm i -D vite;  npx vite
来源：http://hz.cucudq.cn/gtdbwbtgom.html

[U119] JS：生产构建
来源：http://hz.yvedp.cn/gtjlbnghmf.html

npx vite build
来源：http://hz.birdmap.top/gtspyiuhir.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gzhubu.top/gtogtwdysn.html

import.meta.env.VITE_API_URL
来源：http://hz.sufxvd.cn/gtiqnfyqof.html

================================================================================
来源：http://hz.sweek.top/gtrcpmnpev.html

统计汇总
来源：http://hz.xziqi.cn/gtxhcestzv.html

================================================================================
来源：http://hz.cucudq.cn/gtuozzvadl.html

按语言统计（条）：
来源：http://hz.gaohongyu789.top/gtptsyawgo.html

Python ......... 252
来源：http://hz.chenlongwang.top/gtumlmxtoz.html

PHP ............ 252
来源：http://hz.sxryk.cn/gtotjxlvvd.html

JavaScript ..... 252
来源：http://hz.aibaodan.cn/gtuqoikeva.html

TypeScript ..... 212
来源：http://hz.jinghuilouyu.cn/gtgpetahou.html

Java ........... 212
来源：http://hz.tanke756.top/gtzidienso.html

Go ............. 212
来源：http://hz.ywan-chungtsiang.top/gttxtmyvca.html

Ruby ........... 212
来源：http://hz.nanxinkj.top/gtljrcquxg.html

C# ............. 212
来源：http://hz.zhiwuduotai.top/gtaiugufgf.html

C .............. 30
来源：http://hz.daxiang520.top/gtdbeydodx.html

C++ ............ 30
来源：http://hz.jyoumei.cn/gtrlbhdbhl.html

SQL ............ 90
来源：http://hz.jianghu66.top/gtepvcdihm.html

Bash ........... 80
来源：http://hz.ivvv.top/gtfzmvxjzg.html

Kotlin ......... 15
来源：http://hz.cucudq.cn/gtaudryked.html

Swift .......... 15
来源：http://hz.jqgufenzy.top/gtrvolniwv.html

Lua ............ 10
来源：http://hz.zhaomingkeji.xyz/gtdsdmiewe.html

Perl ........... 10
来源：http://hz.c1oappe.top/gtvucuhhiv.html

Scala .......... 10
来源：http://hz.hammf.cn/gtrsjbeole.html

------------------------------------
来源：http://hz.tianlin.xyz/gtukvimymb.html

合计 ........... 2106 条
来源：http://hz.yangfankeji.com/gtkoxgqjlb.html

按章节统计：
来源：http://hz.zhiwuduotai.top/gtbgfizkka.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cucudq.cn/gtnhvouxia.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtvjywhdwn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtnpkzwwap.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtrksfzvic.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sweek.top/gtwwxpxscu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ywan-chungtsiang.top/gttezkhjjm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtqodvwrmx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jlsjyb.cn/gtcrpqzafo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtmknxbsip.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gaohongyu789.top/gtxynjezso.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtjdcifssi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtxrldfpkx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtkdsosmwq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangtech.top/gtsaxumjyk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yj20258.top/gtrjmkbltt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtqtngjmuz.html

Q SQL 专题                              90
来源：http://hz.sweek.top/gtrhiesyhp.html

R Bash 专题                             80
来源：http://hz.shzxlz.cn/gtepxwlwsh.html

S C / C++ 专题                          60
来源：http://hz.feifeiyinyue.top/gtkdlubmpa.html

T 其他语言补充                          60
来源：http://hz.gzhubu.top/gtysmxyxpe.html

U 高频实用片段                         120
来源：http://hz.pycfn.com/gtpopstjzx.html

------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtzzggrlst.html

合计                                  2106 条
来源：http://hz.cucudq.cn/gtonxbkrjr.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtzjhisfyd.html

使用提醒
来源：http://hz.hfpthk.cn/gtixjwbshh.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gtghdloscp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yj202588.top/gtwfzodaco.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yongpay.top/gtxtxdcbkb.html


<!-- 参考信息 -->