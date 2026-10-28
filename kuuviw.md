代发 wailian999

[U11] Py：生成器表达式
来源：http://hz.kuanghao11.cn/gtntfxwkeq.html

(x * 2 for x in arr)
来源：http://hz.sweek.top/gtndyabiym.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.dianchejie.cn/gtbqhelaki.html

Counter(arr).most_common(3)
来源：http://hz.yonumen.top/gtwktpbsqg.html

[U13] Py：固定长度队列
来源：http://hz.yangfankeji.com/gtfmhgfdaw.html

deque(maxlen=10)
来源：http://hz.sufxvd.cn/gtvdmlczoz.html

[U14] Py：分组收集到列表
来源：http://hz.ybcxt.top/gtzgvnfkzi.html

defaultdict(list)
来源：http://hz.yanxiufei.cn/gtrhiksggs.html

[U15] Py：高精度计时
来源：http://hz.hnqzz.top/gtqnvvnccj.html

t = time.perf_counter()
来源：http://hz.yuxming.cn/gtwovasxmb.html

[U16] Py：命令行参数解析
来源：http://hz.kuanghao11.cn/gtnejctpqy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.dashuyun.cn/gtyanbmyxo.html

[U17] Py：初始化日志
来源：http://hz.wangdashe.top/gttfabafdt.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.tanke756.top/gtwprpkfcq.html

[U18] Py：预编译正则
来源：http://hz.xziqi.cn/gtlbddupwd.html

pat = re.compile(r"\d+")
来源：http://hz.wangshuangyany.cn/gtamkzjupg.html

[U19] Py：正则替换带回调
来源：http://hz.yj20258.top/gtvorsdzzs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shuidangran.top/gtigazkuiu.html

[U20] Py：缓存函数结果
来源：http://hz.cheryme.top/gtlohgpwzv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.chenjidiqi.icu/gthflwlodx.html

[U21] Py：自定义上下文管理器
来源：http://hz.guowangkeji.top/gtopmeludd.html

@contextlib.contextmanager
来源：http://hz.meibo888.top/gtdhitlorc.html

[U22] Py：矩阵转置
来源：http://hz.hnqzz.top/gtyrukitjl.html

list(zip(*m))
来源：http://hz.shanyushiyangkeji.top/gtopdnamhs.html

[U23] Py：分块读取大文件
来源：http://hz.fengsongda.top/gtwnmxdmtt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.meibo888.top/gtwgzppwtk.html

[U24] Py：路径操作
来源：http://hz.0kj1m.cn/gtwtunczkn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.svipenyu.cn/gtejxngzgn.html

[U25] Py：CSV 按字典读
来源：http://hz.ydzc1.top/gtvoghpyeg.html

csv.DictReader(f)
来源：http://hz.yvedp.cn/gtpxuyynbg.html

[U26] Py：并发下载
来源：http://hz.gaohongyu789.top/gtfvegddnh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yj20258888.top/gtyxleagou.html

[U27] Py：异步 HTTP
来源：http://hz.zhijiandao.cn/gtwwuyvxbg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zdqjudy.top/gtcxrpiqsw.html

[U28] Py：类型别名
来源：http://hz.xuetiantiany.cn/gtfjjppnsb.html

UserId = int
来源：http://hz.zhijiandao.cn/gtzybfazlu.html

[U29] Py：属性校验
来源：http://hz.cdnleiting.top/gthfreusdp.html

@property 与 @x.setter 配合
来源：http://hz.havefunace.top/gtieqnflmy.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gtzhypxjct.html

@dataclass(slots=True)
来源：http://hz.quarkkingdee.top/gtwitkcwxk.html

[U31] Py：单测
来源：http://hz.0kj1m.cn/gtqietyvgp.html

python -m pytest -q
来源：http://hz.nanxuanxn.top/gtvvwpyuub.html

[U32] Py：代码格式化
来源：http://hz.mhx1999.top/gtxdclpbsa.html

ruff format . && ruff check --fix .
来源：http://hz.meibo888.top/gttypapggs.html

[U33] Py：打包发布
来源：http://hz.jlsjyb.cn/gtmfwvhiel.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cashguo.top/gtzwdefplp.html

[U34] Py：判断编码
来源：http://hz.wangdashe.top/gterxnvedn.html

chardet.detect(raw)
来源：http://hz.yj20258.top/gtumxmbdcf.html

[U35] Py：发送邮件
来源：http://hz.shangyingyoupin.top/gtyrsuzbcl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xingfuxueyuan.xyz/gtldhttwkw.html

[U36] Py：定时任务
来源：http://hz.hysaishi.cn/gtjdvszwli.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258.top/gtmqvmqcem.html

[U37] Py：读写 Excel
来源：http://hz.gzhubu.top/gtjececkbf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj202588.top/gtncigdhxs.html

[U38] Py：获取脚本所在目录
来源：http://hz.gogol.net.cn/gtasltslwa.html

Path(__file__).resolve().parent
来源：http://hz.xingfuxueyuan.xyz/gtlcqghwiy.html

[U39] Py：判断是否在交互环境
来源：http://hz.zdqjudy.top/gthmuobcad.html

sys.stdout.isatty()
来源：http://hz.ydzc1.top/gtxxfuxlhr.html

[U40] Py：打印到标准错误
来源：http://hz.daria6918.cn/gtucfvymzr.html

print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtgdekceeh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jiagoushi.top/gtyanlnndb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhaomingkeji.xyz/gtyyqlydmw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sufxvd.cn/gtvyigjlrk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.andypj.xyz/gtsqiofmal.html

[U43] PHP：声明命名空间
来源：http://hz.svipenyu.cn/gtbvmswnpn.html

namespace App\Http;
来源：http://hz.jqgufenzy.top/gtyduaccsl.html

[U44] PHP：开启严格类型
来源：http://hz.gaohongyu789.top/gtcclfclth.html

declare(strict_types=1);
来源：http://hz.yongpay.top/gtggzabtsi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuanzhike.top/gtigqkkzoa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtbqtwckey.html

[U46] PHP：可空类型
来源：http://hz.fengsongda.top/gthxltmmdr.html

?string $name = null
来源：http://hz.wangdashe.top/gtwjnhecda.html

[U47] PHP：联合类型
来源：http://hz.chenjidiqi.icu/gtrkdodtsm.html

int|string $id
来源：http://hz.ivvv.top/gtufjcbjso.html

[U48] PHP：纯枚举
来源：http://hz.tianlin.xyz/gtkjhmptzm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.kuanghao11.cn/gtfcbdocbe.html

[U49] PHP：只读属性
来源：http://hz.yonumen.top/gtyslwrlgr.html

public readonly string $name
来源：http://hz.xinyue.icu/gtcmsgvsxq.html

[U50] PHP：构造器属性提升
来源：http://hz.ydzc1.top/gtdssirnny.html

public function __construct(private int $id) {}
来源：http://hz.jianghu66.top/gtplawsjoi.html

[U51] PHP：数组解构
来源：http://hz.mhx1999.top/gtqyhootaa.html

[$a, $b] = $arr;
来源：http://hz.cdnleiting.top/gtnbvobfje.html

[U52] PHP：箭头函数
来源：http://hz.haohaochexian.top/gtvouyaysp.html

$double = fn($x) => $x * 2;
来源：http://hz.xylfe.cn/gtbilsvcuw.html

[U53] PHP：空合并运算符
来源：http://hz.sxryk.cn/gtnkntgqwo.html

$v = $a ?? $b ?? "default";
来源：http://hz.ehwqpu.com/gtkhvxzfkn.html

[U54] PHP：空安全调用
来源：http://hz.zhoulong.xyz/gtqbrtvoqe.html

$obj?->method()
来源：http://hz.zhijiandao.cn/gtfybrmktu.html

[U55] PHP：match 表达式
来源：http://hz.316326.xyz/gtbgwcuzza.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj202588.top/gtriwdsleh.html

[U56] PHP：命名参数
来源：http://hz.zhijiandao.cn/gtbmlwahvk.html

f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtpawfafjv.html

[U57] PHP：字符串插值
来源：http://hz.haohaochexian.top/gtnyvrktxw.html

"值: {$a}"
来源：http://hz.zdqjudy.top/gtljvhdnom.html

[U58] PHP：数组三件套
来源：http://hz.zhixingplan.top/gtrimohizu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.nanxinkj.top/gtcrndglpf.html

[U59] PHP：自定义排序
来源：http://hz.chenzaomai.com/gtuyluphbr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.svipenyu.cn/gtmsiwhdol.html

[U60] PHP：JSON 编解码
来源：http://hz.cucudq.cn/gtlpnvhpng.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.fzhhl.top/gttmwipvlj.html

[U61] PHP：正则
来源：http://hz.jinghuilouyu.cn/gtzrrghzfc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gthfydmrdw.html

[U62] PHP：日期对象
来源：http://hz.guannengcc.top/gtrctdmwtt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hammf.cn/gtmflfnreg.html

[U63] PHP：文件读写
来源：http://hz.quarkkingdee.top/gtasyfwerk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258888.top/gtwzkxhyee.html

[U64] PHP：目录遍历
来源：http://hz.hywenlv.cn/gtvonnxuff.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yuanzhike.top/gtlbloanko.html

[U65] PHP：会话
来源：http://hz.ydzc1.top/gtgtxfhknw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hammf.cn/gtnniffhzz.html

[U66] PHP：设置 Cookie
来源：http://hz.yongpay.top/gtfwhfgzsi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yanxiufei.cn/gthplvspvx.html

[U67] PHP：处理文件上传
来源：http://hz.hammf.cn/gtwcsfzzlu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.iojbl.cn/gtkzyviixb.html

[U68] PHP：PDO 连接
来源：http://hz.jinqigufen.top/gtxurdmrjo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.snrcjt.cn/gtjxazwkpq.html

[U69] PHP：PDO 预处理
来源：http://hz.tian-w.cn/gtlqhxwgio.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jqgufenzy.top/gtswotvqfv.html

[U70] PHP：PDO 事务
来源：http://hz.aizwys.cn/gtcppqfrrs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.andypj.xyz/gtuhplgslc.html

[U71] PHP：抛出异常
来源：http://hz.jinyuanbaomall.cn/gtrsaxahph.html

throw new RuntimeException("失败", 500);
来源：http://hz.yuanzhike.top/gtgdlyiihm.html

[U72] PHP：写错误日志
来源：http://hz.zhijiandao.cn/gtzomyxtbu.html

error_log("失败: " . $e->getMessage());
来源：http://hz.nanxinkj.top/gtnvaqdory.html

[U73] PHP：读取 ini 配置
来源：http://hz.xziqi.cn/gtbjvaajqp.html

parse_ini_file("config.ini", true)
来源：http://hz.jqgfzy.top/gtksahdpgb.html

[U74] PHP：读取环境变量
来源：http://hz.chenlongwang.top/gtfqirhjqv.html

getenv("APP_ENV") ?: "production"
来源：http://hz.quarkkingdee.top/gtblvwjkzn.html

[U75] PHP：依赖注入
来源：http://hz.ppjwa.cn/gtxnhtoins.html

composer require psr/container
来源：http://hz.havefunace.top/gtgftfoter.html

[U76] PHP：简单路由
来源：http://hz.316326.xyz/gtanptmanc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cashguo.top/gtmpltbjep.html

[U77] PHP：模板渲染
来源：http://hz.nanxinkj.top/gttbbohpid.html

composer require twig/twig
来源：http://hz.redwolf501.top/gtqugyqgsp.html

[U78] PHP：单元测试
来源：http://hz.gaohongyu789.top/gtrzjbwwau.html

composer require --dev phpunit/phpunit
来源：http://hz.nanxuanxn.top/gtbiychgwq.html

[U79] PHP：静态分析
来源：http://hz.pengpengdd.cyou/gtiwblegmd.html

composer require --dev phpstan/phpstan
来源：http://hz.ywan-chungtsiang.top/gtnkswbksd.html

[U80] PHP：代码规范修复
来源：http://hz.ydjk.org.cn/gtpnigivku.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yanxiufei.cn/gtopeggwlv.html

[U81] JS：初始化项目
来源：http://hz.xuanzx.com/gtybnghdca.html

npm init -y;  npm i express
来源：http://hz.hongshengwenyu.top/gtijddrwas.html

[U82] JS：package.json 脚本
来源：http://hz.meibo888.top/gtfjaqcsus.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.chenlongwang.top/gtsegabjjs.html

[U83] JS：ES Module 导入导出
来源：http://hz.meibo888.top/gtiytxlhnw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.fengsongda.top/gtmjkjqqzv.html

[U84] JS：CommonJS 写法
来源：http://hz.zdqjudy.top/gtazvjwgoi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.dianchejie.cn/gtcalzkbnl.html

[U85] JS：可选链
来源：http://hz.jqgufenzy.top/gtwfvuozpl.html

a?.b?.c
来源：http://hz.sysykeji.top/gtrndfsfik.html

[U86] JS：空值合并
来源：http://hz.jianghu66.top/gthfjlmgao.html

a ?? b
来源：http://hz.jqgufenzy.top/gtrmglifzt.html

[U87] JS：解构默认值
来源：http://hz.xuanzx.com/gtvncielcd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.redwolf501.top/gtgzbvocda.html

[U88] JS：对象展开合并
来源：http://hz.shangyingyoupin.top/gtnrclcmyq.html

{ ...a, ...b }
来源：http://hz.gzhubu.top/gtcwnayzvc.html

[U89] JS：数组去重
来源：http://hz.xuanzx.com/gttkgdcxai.html

[...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtorirucza.html

[U90] JS：数字数组排序
来源：http://hz.zhengqikj.top/gtluxulpfk.html

[...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtmytagzwq.html

[U91] JS：对象键值遍历
来源：http://hz.hammf.cn/gtgpsfbwbh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.52xcode.cn/gtdkyaxrqc.html

[U92] JS：深拷贝
来源：http://hz.yuanzhike.top/gtudjjcwei.html

structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtadnekvog.html

[U93] JS：模板字符串
来源：http://hz.dashuyun.cn/gtygdceotn.html

`共 ${n} 条`
来源：http://hz.ppjwa.cn/gtncjbroeq.html

[U94] JS：箭头函数
来源：http://hz.yonumen.top/gtxdvqtkkj.html

const double = x => x * 2;
来源：http://hz.tianlin.xyz/gtjuvtspim.html

[U95] JS：Promise 包装
来源：http://hz.0kj1m.cn/gtcponaqmc.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxuanxn.top/gtwmkbcstg.html

[U96] JS：async/await 与异常
来源：http://hz.xuanzx.com/gtzxucgjrb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtvtsycvmk.html

[U97] JS：并发请求
来源：http://hz.sysykeji.top/gtefcjefag.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gthujmgjty.html

[U98] JS：fetch 带 JSON
来源：http://hz.gogol.net.cn/gtmsmwbcdg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.0kj1m.cn/gtghrfyzmt.html

[U99] JS：事件监听
来源：http://hz.dianchejie.cn/gtyexyliac.html

el.addEventListener("click", e => {})
来源：http://hz.gzhubu.top/gtanedqibm.html

[U100] JS：DOM 查询
来源：http://hz.zdqjudy.top/gtmfjchgsb.html

document.querySelector(".item")
来源：http://hz.shzxlz.cn/gtaaintpcz.html

[U101] JS：classList 操作
来源：http://hz.birdmap.top/gtuutukcyg.html

el.classList.toggle("active")
来源：http://hz.birdmap.top/gtllydxvjb.html

[U102] JS：本地存储
来源：http://hz.nwbrower.top/gtaeflwoel.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yueranfly.top/gtpxgnfpqn.html

[U103] JS：定时器
来源：http://hz.nwbrower.top/gtidhxjvcb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.kuanghao11.cn/gtaqshndhu.html

[U104] JS：防抖
来源：http://hz.hnxiangtu.top/gtxtfjjnge.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtuhedtsxy.html

[U105] JS：节流
来源：http://hz.hnqzz.top/gtovzutkfg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ybcxt.top/gtgpwgfqal.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gthzggflgr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.chenzaomai.com/gtwmsomgre.html

[U107] JS：数字千分位
来源：http://hz.pycfn.com/gttrjrbaid.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.andypj.xyz/gtpevvysci.html

[U108] JS：随机整数
来源：http://hz.jinqigfzy.top/gtdzryfhyl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ydzc1.top/gtqccamofj.html

[U109] JS：数组分组
来源：http://hz.nanxuanxn.top/gtpjgjxdeu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtujekegti.html

[U110] JS：数组分块
来源：http://hz.hammf.cn/gtrocscsjf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.vqdsnc.cn/gtrbejmuxs.html

[U111] JS：对象转 Map
来源：http://hz.nanxuanxn.top/gtgckndmcp.html

new Map(Object.entries(obj))
来源：http://hz.ppjwa.cn/gtjzulxeuz.html

[U112] JS：字符串补位
来源：http://hz.hongshengwenyu.top/gttxpghllf.html

"7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtvqomjuvk.html

[U113] JS：正则替换全部
来源：http://hz.ydjk.org.cn/gtkwvdszbe.html

s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtnnmxadco.html

[U114] JS：JSON 深比较
来源：http://hz.jqgfzy.top/gtgkcxffuq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nwbrower.top/gtbvdvkfxa.html

[U115] JS：生成 UUID
来源：http://hz.gaohongyu789.top/gtwskkhjhw.html

crypto.randomUUID()
来源：http://hz.9152youxi.cn/gtniuhwzdc.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sysykeji.top/gtyrevmdua.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj20258888.top/gtxdxvivul.html

[U117] JS：单元测试
来源：http://hz.ivvv.top/gtjahygtxi.html

npm i -D vitest;  npx vitest
来源：http://hz.xinyue.icu/gtuibejbfs.html

[U118] JS：开发服务器
来源：http://hz.svipenyu.cn/gthdejfaus.html

npm i -D vite;  npx vite
来源：http://hz.zhiwuduotai.top/gtvplaxkld.html

[U119] JS：生产构建
来源：http://hz.cdnleiting.top/gtnwvlpyos.html

npx vite build
来源：http://hz.yuxming.cn/gtzkplvypp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yongpay.top/gtanvqzcsw.html

import.meta.env.VITE_API_URL
来源：http://hz.shangyingyoupin.top/gtuuszzzdv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvnnrlpny.html

统计汇总
来源：http://hz.daria6918.cn/gttjkxwuhj.html

================================================================================
来源：http://hz.sweek.top/gthemtcwph.html

按语言统计（条）：
来源：http://hz.tian-w.cn/gtfvmgcksb.html

Python ......... 252
来源：http://hz.aibaodan.cn/gtajsxkqpw.html

PHP ............ 252
来源：http://hz.bjfxy.top/gtzfmctrvy.html

JavaScript ..... 252
来源：http://hz.ehwqpu.com/gtjtakwvvn.html

TypeScript ..... 212
来源：http://hz.tian-w.cn/gtxpzxxiwl.html

Java ........... 212
来源：http://hz.mhx1999.top/gtyiygqist.html

Go ............. 212
来源：http://hz.hywenlv.cn/gtpmjwtuvi.html

Ruby ........... 212
来源：http://hz.andypj.xyz/gtvhszmcrm.html

C# ............. 212
来源：http://hz.svipenyu.cn/gtwrunvbcx.html

C .............. 30
来源：http://hz.redwolf501.top/gtohlczbko.html

C++ ............ 30
来源：http://hz.pycfn.com/gttpohzifi.html

SQL ............ 90
来源：http://hz.jiagoushi.top/gtbuotexfh.html

Bash ........... 80
来源：http://hz.shanyushiyangkeji.top/gtfvycghbq.html

Kotlin ......... 15
来源：http://hz.yongpay.top/gtbvlcmxif.html

Swift .......... 15
来源：http://hz.aibaodan.cn/gtlgrpsqwt.html

Lua ............ 10
来源：http://hz.zycfv.cn/gtkfubcnad.html

Perl ........... 10
来源：http://hz.zhaomingkeji.xyz/gtzjdwuswg.html

Scala .......... 10
来源：http://hz.iojbl.cn/gtjofffmsb.html

------------------------------------
来源：http://hz.sysykeji.top/gtkhitmlfn.html

合计 ........... 2106 条
来源：http://hz.xylfe.cn/gternrnlsv.html

按章节统计：
来源：http://hz.kuanghao11.cn/gtimlzknoj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gtuuvqlgky.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gtarzramoi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtbbzmijzu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinyuanbaomall.cn/gtohngmgjm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinghuilouyu.cn/gtyndcwdvv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shzxlz.cn/gtglopnsir.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258888.top/gtdyerliqn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangdashe.top/gthesclxlh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtrrlomlsw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.0kj1m.cn/gtwaukhjbz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtraixrqeb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtejkdjmek.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtskrjgjis.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zycfv.cn/gtkjsabhme.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.snrcjt.cn/gtwlkpgcyi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtqqachqry.html

Q SQL 专题                              90
来源：http://hz.hfpthk.cn/gtjswolzaq.html

R Bash 专题                             80
来源：http://hz.ehwqpu.com/gtbyexqyss.html

S C / C++ 专题                          60
来源：http://hz.yangfankeji.com/gthqutpdyc.html

T 其他语言补充                          60
来源：http://hz.haohaochexian.top/gtyyzutdgf.html

U 高频实用片段                         120
来源：http://hz.cdnleiting.top/gtubbnpdcb.html

------------------------------------
来源：http://hz.tanke756.top/gtxlglwmzq.html

合计                                  2106 条
来源：http://hz.bjfxy.top/gtubqalprf.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtykpagvrt.html

使用提醒
来源：http://hz.bjfxy.top/gtfrzfumsn.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtfnrywpmi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xinyue.icu/gtrtjaxfnp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.snrcjt.cn/gtysxhains.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.tianlin.xyz/gtsnlduqez.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhengqikj.top/gtqlcbwokk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhixingplan.top/gtwcofzhff.html

—— 文件结束 ——
来源：http://hz.pycfn.com/gthgneasrp.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqhoedzpc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.redwolf501.top/gtsxwgfdda.html

Common Programming Examples Cheat Book
来源：http://hz.yj202588.top/gtbmxpfiko.html

================================================================================
来源：http://hz.yongpay.top/gttkndzlrg.html

【收录内容】
来源：http://hz.ydzc1.top/gtqvvrheve.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.daxiang520.top/gtfpkqhokz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jianghu66.top/gtdzoabwck.html

SQL · Bash · C · C++
来源：http://hz.zhengqikj.top/gtzyjwpspd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jianghu66.top/gtzrhxwjwn.html

【使用说明】
来源：http://hz.jinghuilouyu.cn/gtdvsijyea.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yj202588.top/gtgmwacgvz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhaomingkeji.xyz/gthujjzcsr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.wangshuangyany.cn/gtfjkypaot.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.316326.xyz/gtcsqklxrc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.kuanghao11.cn/gtxfsdybzn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gogol.net.cn/gtozvvlxao.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.52xcode.cn/gtawmommjp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.tianlin.xyz/gtvygjdddu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.gzhubu.top/gtszzfzvtx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhixingplan.top/gttsdvgasy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhijiandao.cn/gtxiduegaw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hywenlv.cn/gtknyszzjx.html

【文件统计】
来源：http://hz.jinqigfzy.top/gtqnonoksa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.iojbl.cn/gtgkxakszt.html


<!-- 参考信息 -->