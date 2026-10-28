代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.svipenyu.cn/gtzihrxjij.html

[T59] Scala：循环
来源：http://hz.hfpthk.cn/gtiubkknza.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnxiangtu.top/gtfamqoyxo.html

[T60] Scala：折叠
来源：http://hz.yueranfly.top/gtdxlllseu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258888.top/gtrlskxxhh.html

================================================================================
来源：http://hz.guannengcc.top/gthexzasrc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yonumen.top/gtnxmjrtpw.html

================================================================================
来源：http://hz.jianghu66.top/gtxleliraw.html

[U01] Py：创建虚拟环境
来源：http://hz.chenjidiqi.icu/gteiyoqdaz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinyuanbaomall.cn/gtetidplln.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shangyingyoupin.top/gtkqsahwqv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnxiangtu.top/gtdbbncdvm.html

[U03] Py：加载 .env 配置
来源：http://hz.jiagoushi.top/gtmlhfzjgp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenjidiqi.icu/gtsuwabsgm.html

[U04] Py：变量调试打印
来源：http://hz.gotoacloud.top/gtnxshflez.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gaohongyu789.top/gtqpxrymwo.html

[U05] Py：列表去重且保序
来源：http://hz.pengpengdd.cyou/gtyesecgln.html

list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gtcosxqjvu.html

[U06] Py：合并两个字典
来源：http://hz.tian-w.cn/gttjmozglx.html

{**a, **b}
来源：http://hz.zhijiandao.cn/gtsjveeild.html

[U07] Py：反转字典键值
来源：http://hz.hammf.cn/gtnjlhlulc.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gttuxszbyc.html

[U08] Py：展平二维列表
来源：http://hz.jqgufenzy.top/gtjclrjhuj.html

[y for x in nested for y in x]
来源：http://hz.316326.xyz/gtfnmkxewi.html

[U09] Py：字典取最大值的键
来源：http://hz.wangdashe.top/gtnpfyolcm.html

max(d, key=d.get)
来源：http://hz.shanyushiyangkeji.top/gtvysdfttz.html

[U10] Py：按值排序字典
来源：http://hz.xziqi.cn/gttbfrhzjj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xziqi.cn/gtzlskoera.html

[U11] Py：生成器表达式
来源：http://hz.jianghu66.top/gtlvkxosyt.html

(x * 2 for x in arr)
来源：http://hz.smart0.xyz/gthnkfkjkg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jqgufenzy.top/gtdeencmqv.html

Counter(arr).most_common(3)
来源：http://hz.wangshuangyany.cn/gtdduuoved.html

[U13] Py：固定长度队列
来源：http://hz.316326.xyz/gtwijhjjtv.html

deque(maxlen=10)
来源：http://hz.tanke756.top/gtowtqmxdb.html

[U14] Py：分组收集到列表
来源：http://hz.mhx1999.top/gtimfinoxv.html

defaultdict(list)
来源：http://hz.meibo888.top/gtxuloprlb.html

[U15] Py：高精度计时
来源：http://hz.yanxiufei.cn/gtupxqhrfd.html

t = time.perf_counter()
来源：http://hz.yanxiufei.cn/gtzqwokkai.html

[U16] Py：命令行参数解析
来源：http://hz.0kj1m.cn/gtxkoeqvoq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.bjfxy.top/gtfgmdoaey.html

[U17] Py：初始化日志
来源：http://hz.kuanghao11.cn/gtsfikbcnn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nanxuanxn.top/gtjhvpwrxb.html

[U18] Py：预编译正则
来源：http://hz.gzhubu.top/gtylghxyof.html

pat = re.compile(r"\d+")
来源：http://hz.cheryme.top/gtyjjvetue.html

[U19] Py：正则替换带回调
来源：http://hz.c1oappe.top/gtxlvykdrh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.smart0.xyz/gtlmbiwjxz.html

[U20] Py：缓存函数结果
来源：http://hz.xuanzx.com/gtbnbpgyqb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xinyue.icu/gtpnnvlwat.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinqigufen.top/gtnhblpuww.html

@contextlib.contextmanager
来源：http://hz.hfpthk.cn/gtsqyejmxa.html

[U22] Py：矩阵转置
来源：http://hz.wangshuangyany.cn/gteqbzwoun.html

list(zip(*m))
来源：http://hz.9152youxi.cn/gtklbltaxv.html

[U23] Py：分块读取大文件
来源：http://hz.xziqi.cn/gtvxcyvbfu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zdqjudy.top/gtdylzcpzt.html

[U24] Py：路径操作
来源：http://hz.hysaishi.cn/gtytfnyonh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenzaomai.com/gtemvzwlok.html

[U25] Py：CSV 按字典读
来源：http://hz.jyoumei.cn/gtjtmjmamu.html

csv.DictReader(f)
来源：http://hz.hfpthk.cn/gtvhpxukgi.html

[U26] Py：并发下载
来源：http://hz.hywenlv.cn/gtwbjknulv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dashuyun.cn/gtkxpzvtkq.html

[U27] Py：异步 HTTP
来源：http://hz.daxiang520.top/gtnwyaffkf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.smart0.xyz/gtjzimjdos.html

[U28] Py：类型别名
来源：http://hz.zdqjudy.top/gtahzagimm.html

UserId = int
来源：http://hz.yj20258.top/gtzmuaqoup.html

[U29] Py：属性校验
来源：http://hz.yj202588.top/gtthkdxorr.html

@property 与 @x.setter 配合
来源：http://hz.hywenlv.cn/gttgkuxxnw.html

[U30] Py：数据类
来源：http://hz.ydjk.org.cn/gtjtjocdir.html

@dataclass(slots=True)
来源：http://hz.jyoumei.cn/gtncgxavtk.html

[U31] Py：单测
来源：http://hz.hysaishi.cn/gtodxsbeir.html

python -m pytest -q
来源：http://hz.zdqjudy.top/gtlvgvtsgr.html

[U32] Py：代码格式化
来源：http://hz.wangdashe.top/gtorwdlwts.html

ruff format . && ruff check --fix .
来源：http://hz.zhoulong.xyz/gtdqkcdour.html

[U33] Py：打包发布
来源：http://hz.zdqjudy.top/gtqcztswpq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gaohongyu789.top/gtmfluvhnr.html

[U34] Py：判断编码
来源：http://hz.sxryk.cn/gteisfqheq.html

chardet.detect(raw)
来源：http://hz.tanke756.top/gtbhtiyhiv.html

[U35] Py：发送邮件
来源：http://hz.guowangkeji.top/gtpghixkfw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sysykeji.top/gtxzuirznc.html

[U36] Py：定时任务
来源：http://hz.shangyingyoupin.top/gtfjwugapr.html

schedule.every(10).minutes.do(job)
来源：http://hz.redwolf501.top/gtcmfwbzle.html

[U37] Py：读写 Excel
来源：http://hz.cdnleiting.top/gtnhdgpueo.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hfpthk.cn/gtjqbmoowp.html

[U38] Py：获取脚本所在目录
来源：http://hz.ppjwa.cn/gtrxlqikgm.html

Path(__file__).resolve().parent
来源：http://hz.jlsjyb.cn/gtvqkvzvwt.html

[U39] Py：判断是否在交互环境
来源：http://hz.haohaochexian.top/gtnypwqnar.html

sys.stdout.isatty()
来源：http://hz.hnqzz.top/gtetvnqphf.html

[U40] Py：打印到标准错误
来源：http://hz.c1oappe.top/gtsnhfxelf.html

print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gtiynjmskd.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.redwolf501.top/gtfmqcftvf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xylfe.cn/gtepdzcxqm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.fzhhl.top/gtngnvumot.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pengpengdd.cyou/gtxiegcyil.html

[U43] PHP：声明命名空间
来源：http://hz.aibaodan.cn/gteqtzaris.html

namespace App\Http;
来源：http://hz.birdmap.top/gtlfbicrpn.html

[U44] PHP：开启严格类型
来源：http://hz.ydjk.org.cn/gtrbhexfmn.html

declare(strict_types=1);
来源：http://hz.hfpthk.cn/gtcccaulnz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shuidangran.top/gtlgxeupaf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtexmyknaw.html

[U46] PHP：可空类型
来源：http://hz.sxryk.cn/gttigakhuz.html

?string $name = null
来源：http://hz.chenzaomai.com/gttqyxfose.html

[U47] PHP：联合类型
来源：http://hz.0kj1m.cn/gtrjyxlait.html

int|string $id
来源：http://hz.jinqigufen.top/gtbvyzkwky.html

[U48] PHP：纯枚举
来源：http://hz.gaohongyu789.top/gtmmuryrnj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.dianchejie.cn/gtrljkujse.html

[U49] PHP：只读属性
来源：http://hz.hnqzz.top/gtjzxthmji.html

public readonly string $name
来源：http://hz.bjfxy.top/gtdiuqjoni.html

[U50] PHP：构造器属性提升
来源：http://hz.ydzc1.top/gtekziquao.html

public function __construct(private int $id) {}
来源：http://hz.guowangkeji.top/gtgmcsdakx.html

[U51] PHP：数组解构
来源：http://hz.snrcjt.cn/gtzyxyjwqv.html

[$a, $b] = $arr;
来源：http://hz.ppjwa.cn/gtnvnachsn.html

[U52] PHP：箭头函数
来源：http://hz.pycfn.com/gtjxewiemj.html

$double = fn($x) => $x * 2;
来源：http://hz.jinyuanbaomall.cn/gtrktylucu.html

[U53] PHP：空合并运算符
来源：http://hz.gaohongyu789.top/gtcyespdff.html

$v = $a ?? $b ?? "default";
来源：http://hz.zdqjudy.top/gtebqgmjhh.html

[U54] PHP：空安全调用
来源：http://hz.jianghu66.top/gtfddmtalg.html

$obj?->method()
来源：http://hz.yonumen.top/gtyvqjiosx.html

[U55] PHP：match 表达式
来源：http://hz.chenjidiqi.icu/gtilgufibk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj202588.top/gtpccfbnct.html

[U56] PHP：命名参数
来源：http://hz.nanxuanxn.top/gtmozfdrov.html

f(a: 1, b: 2)
来源：http://hz.dashuyun.cn/gtrlxqnxus.html

[U57] PHP：字符串插值
来源：http://hz.meibo888.top/gtysapduxy.html

"值: {$a}"
来源：http://hz.gzhubu.top/gtecjgdcwj.html

[U58] PHP：数组三件套
来源：http://hz.andypj.xyz/gtgghsdryn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jianghu66.top/gtacyukdkr.html

[U59] PHP：自定义排序
来源：http://hz.zhaomingkeji.xyz/gtrvwuvoxm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jianghu66.top/gttitocyny.html

[U60] PHP：JSON 编解码
来源：http://hz.nwbrower.top/gtzhqxwbap.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhixingplan.top/gtbcdvsdzb.html

[U61] PHP：正则
来源：http://hz.jiagoushi.top/gtoxnpuduq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.c1oappe.top/gtvzcktneh.html

[U62] PHP：日期对象
来源：http://hz.chenzaomai.com/gtgbxgiofk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.fengsongda.top/gtqpfdocwr.html

[U63] PHP：文件读写
来源：http://hz.jinyuanbaomall.cn/gtojeqnaej.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hywenlv.cn/gtsvjegzxb.html

[U64] PHP：目录遍历
来源：http://hz.gzhubu.top/gtiokpjxog.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zycfv.cn/gtcmzevetn.html

[U65] PHP：会话
来源：http://hz.nwbrower.top/gtdqscctni.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.9152youxi.cn/gtaedgjjyq.html

[U66] PHP：设置 Cookie
来源：http://hz.zhengqikj.top/gtgxpurkml.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.tianlin.xyz/gtrhahxrwx.html

[U67] PHP：处理文件上传
来源：http://hz.smart0.xyz/gtoxaisbom.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.kuanghao11.cn/gtjuypptff.html

[U68] PHP：PDO 连接
来源：http://hz.cdnleiting.top/gtdhurlthm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.pycfn.com/gtbxuilwwb.html

[U69] PHP：PDO 预处理
来源：http://hz.yj20258.top/gtzfijseai.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.pengpengdd.cyou/gtwuvoigzj.html

[U70] PHP：PDO 事务
来源：http://hz.snrcjt.cn/gtbcyjcbsn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.chenjidiqi.icu/gtsefxxgmv.html

[U71] PHP：抛出异常
来源：http://hz.jiagoushi.top/gtiaxtnnwk.html

throw new RuntimeException("失败", 500);
来源：http://hz.cqqwz.cn/gtrlxcxmge.html

[U72] PHP：写错误日志
来源：http://hz.yangfankeji.com/gtprvnttla.html

error_log("失败: " . $e->getMessage());
来源：http://hz.nanxuanxn.top/gtyftbcsvw.html

[U73] PHP：读取 ini 配置
来源：http://hz.redwolf501.top/gtodtoqfea.html

parse_ini_file("config.ini", true)
来源：http://hz.hongshengwenyu.top/gtqjerrwlr.html

[U74] PHP：读取环境变量
来源：http://hz.fengsongda.top/gtaezyfwcg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shanyushiyangkeji.top/gtnhbhznmz.html

[U75] PHP：依赖注入
来源：http://hz.pycfn.com/gttosxvhpf.html

composer require psr/container
来源：http://hz.cheryme.top/gtohpccnhw.html

[U76] PHP：简单路由
来源：http://hz.yongpay.top/gtfnnhnqjp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ivvv.top/gtbmfljdiz.html

[U77] PHP：模板渲染
来源：http://hz.xuetiantiany.cn/gtrjivjeze.html

composer require twig/twig
来源：http://hz.dianchejie.cn/gtvxuyhoqb.html

[U78] PHP：单元测试
来源：http://hz.tanke756.top/gtfllwjzlc.html

composer require --dev phpunit/phpunit
来源：http://hz.ywan-chungtsiang.top/gtenyxvovi.html

[U79] PHP：静态分析
来源：http://hz.0kj1m.cn/gtswksmtek.html

composer require --dev phpstan/phpstan
来源：http://hz.xziqi.cn/gtqtgwxrbl.html

[U80] PHP：代码规范修复
来源：http://hz.jlsjyb.cn/gtqnfameag.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.316326.xyz/gtuuxjswqh.html

[U81] JS：初始化项目
来源：http://hz.ivvv.top/gtghzfqjvb.html

npm init -y;  npm i express
来源：http://hz.andypj.xyz/gtjikuxgra.html

[U82] JS：package.json 脚本
来源：http://hz.cdnleiting.top/gtkmwmkmal.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.chenjidiqi.icu/gtgysxmrqj.html

[U83] JS：ES Module 导入导出
来源：http://hz.smart0.xyz/gtliqkyejc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.pengpengdd.cyou/gtqwohxygr.html

[U84] JS：CommonJS 写法
来源：http://hz.zhijiandao.cn/gtjijratzg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jianghu66.top/gtmtwdsylo.html

[U85] JS：可选链
来源：http://hz.52xcode.cn/gtmfilksnr.html

a?.b?.c
来源：http://hz.sufxvd.cn/gtsitgnzzu.html

[U86] JS：空值合并
来源：http://hz.aibaodan.cn/gtwbtuwkkp.html

a ?? b
来源：http://hz.redwolf501.top/gtajotyaye.html

[U87] JS：解构默认值
来源：http://hz.quarkkingdee.top/gtaqafxxrg.html

const { a = 1, b = 2 } = obj;
来源：http://hz.nanxinkj.top/gtetffbtmy.html

[U88] JS：对象展开合并
来源：http://hz.cdnleiting.top/gtkzexztkx.html

{ ...a, ...b }
来源：http://hz.xylfe.cn/gtabsahxhx.html

[U89] JS：数组去重
来源：http://hz.xuanzx.com/gtakjofyvs.html

[...new Set(arr)]
来源：http://hz.hnqzz.top/gtznkjexrw.html

[U90] JS：数字数组排序
来源：http://hz.pycfn.com/gtvpojoddu.html

[...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtoyrqeluz.html

[U91] JS：对象键值遍历
来源：http://hz.cashguo.top/gtlhmcfzvn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.pycfn.com/gtipputubj.html

[U92] JS：深拷贝
来源：http://hz.chenlongwang.top/gtbekotyab.html

structuredClone(obj)
来源：http://hz.52xcode.cn/gtxzwrmlzs.html

[U93] JS：模板字符串
来源：http://hz.zhaomingkeji.xyz/gtjnbkfuga.html

`共 ${n} 条`
来源：http://hz.ivvv.top/gttwfbgdfo.html

[U94] JS：箭头函数
来源：http://hz.hysaishi.cn/gtwycshhdv.html

const double = x => x * 2;
来源：http://hz.dianchejie.cn/gtacfnzodh.html

[U95] JS：Promise 包装
来源：http://hz.aibaodan.cn/gthxgstmjw.html

new Promise((resolve, reject) => {})
来源：http://hz.aibaodan.cn/gtbgafawep.html

[U96] JS：async/await 与异常
来源：http://hz.kuanghao11.cn/gtahalkmqs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtpjzinxwj.html

[U97] JS：并发请求
来源：http://hz.yj202588.top/gtofhvezal.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtfgoqtzsn.html

[U98] JS：fetch 带 JSON
来源：http://hz.jyoumei.cn/gtzsyvxyum.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.birdmap.top/gtuhobwrng.html

[U99] JS：事件监听
来源：http://hz.xinyue.icu/gtcfsmugbb.html

el.addEventListener("click", e => {})
来源：http://hz.smart0.xyz/gthbcihygo.html

[U100] JS：DOM 查询
来源：http://hz.yuanzhike.top/gtjjwixoyd.html

document.querySelector(".item")
来源：http://hz.quarkkingdee.top/gteutfelhb.html

[U101] JS：classList 操作
来源：http://hz.cdnleiting.top/gtomzsrabg.html

el.classList.toggle("active")
来源：http://hz.hysaishi.cn/gtdittpxno.html

[U102] JS：本地存储
来源：http://hz.shangyingyoupin.top/gtvjbapdvl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.redwolf501.top/gtdspuztgj.html

[U103] JS：定时器
来源：http://hz.snrcjt.cn/gtylgexjgt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gzhubu.top/gtjhebvpru.html

[U104] JS：防抖
来源：http://hz.yuanzhike.top/gtabyntjyk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.meibo888.top/gtziuqwrdl.html

[U105] JS：节流
来源：http://hz.yj20258.top/gtojmudnjh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dianchejie.cn/gtelsiwcun.html

[U106] JS：日期格式化
来源：http://hz.dianchejie.cn/gtkvayoeta.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhijiandao.cn/gtceqgqlmf.html

[U107] JS：数字千分位
来源：http://hz.snrcjt.cn/gtkchgqhiz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.dianchejie.cn/gtvzatrnon.html

[U108] JS：随机整数
来源：http://hz.sysykeji.top/gtpoxvfrqk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shzxlz.cn/gtyyuayime.html

[U109] JS：数组分组
来源：http://hz.chenlongwang.top/gtsfvpeudz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtxkwrljtp.html

[U110] JS：数组分块
来源：http://hz.chenzaomai.com/gtvjhysndf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.bjfxy.top/gtsmftzucc.html

[U111] JS：对象转 Map
来源：http://hz.pycfn.com/gtvnhwnhdd.html

new Map(Object.entries(obj))
来源：http://hz.zhoulong.xyz/gthtponkye.html

[U112] JS：字符串补位
来源：http://hz.jqgfzy.top/gtjunrsmpk.html

"7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtbebufgws.html

[U113] JS：正则替换全部
来源：http://hz.shangyingyoupin.top/gtahhspmwz.html

s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtnmudtqaf.html

[U114] JS：JSON 深比较
来源：http://hz.sweek.top/gtouzjfvlq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gtrnjzzqqh.html

[U115] JS：生成 UUID
来源：http://hz.zycfv.cn/gturirpqxm.html

crypto.randomUUID()
来源：http://hz.andypj.xyz/gtayhpnclk.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shangyingyoupin.top/gtnvpkuumw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.0kj1m.cn/gtywzbcowx.html

[U117] JS：单元测试
来源：http://hz.ybcxt.top/gtvinfrohs.html

npm i -D vitest;  npx vitest
来源：http://hz.iojbl.cn/gttcwqgpsg.html

[U118] JS：开发服务器
来源：http://hz.yonumen.top/gtbvsxsqas.html

npm i -D vite;  npx vite
来源：http://hz.wangdashe.top/gtuagvxeuy.html

[U119] JS：生产构建
来源：http://hz.ivvv.top/gtzxavxzhx.html

npx vite build
来源：http://hz.smart0.xyz/gtdxtfujle.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yuxming.cn/gtjzfzplhs.html

import.meta.env.VITE_API_URL
来源：http://hz.zhiwuduotai.top/gtojnnwxnx.html

================================================================================
来源：http://hz.svipenyu.cn/gtjxkobyyg.html

统计汇总
来源：http://hz.fengsongda.top/gtikbmxtso.html

================================================================================
来源：http://hz.cashguo.top/gtvfixvwqj.html

按语言统计（条）：
来源：http://hz.yvedp.cn/gtauezyqjq.html

Python ......... 252
来源：http://hz.shanyushiyangkeji.top/gtowgiovgn.html

PHP ............ 252
来源：http://hz.pycfn.com/gtiskxsclu.html

JavaScript ..... 252
来源：http://hz.aizwys.cn/gtaoezqipa.html

TypeScript ..... 212
来源：http://hz.zycfv.cn/gtrhyuourt.html

Java ........... 212
来源：http://hz.svipenyu.cn/gtfedhyliw.html

Go ............. 212
来源：http://hz.yuxming.cn/gtvtivlqlu.html

Ruby ........... 212
来源：http://hz.guowangkeji.top/gtossheoba.html

C# ............. 212
来源：http://hz.zhijiandao.cn/gtaslrplxs.html

C .............. 30
来源：http://hz.zycfv.cn/gtlbslrzxl.html

C++ ............ 30
来源：http://hz.0kj1m.cn/gtpxtbcdnf.html

SQL ............ 90
来源：http://hz.cqqwz.cn/gtpbaqdbhv.html

Bash ........... 80
来源：http://hz.dashuyun.cn/gtkacphrma.html

Kotlin ......... 15
来源：http://hz.yuxming.cn/gtxcnprihe.html

Swift .......... 15
来源：http://hz.tianlin.xyz/gtlrgjhqns.html

Lua ............ 10
来源：http://hz.vqdsnc.cn/gthptpsvtb.html

Perl ........... 10
来源：http://hz.zhiwuduotai.top/gttsoqqvle.html

Scala .......... 10
来源：http://hz.chenjidiqi.icu/gtdwglhoyz.html

------------------------------------
来源：http://hz.0kj1m.cn/gteefvuhdb.html

合计 ........... 2106 条
来源：http://hz.xuanzx.com/gtfuupfeee.html

按章节统计：
来源：http://hz.jinyuanbaomall.cn/gtwaymsgxj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.andypj.xyz/gtokjsysgl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtrjkvuite.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yonumen.top/gtdkxohvta.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.tanke756.top/gtdbjjsewh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhongyouzk.top/gtmsohskva.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtcfjsihgg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtpodlhkqk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtnypjqnxo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtdynsbnfy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cqqwz.cn/gtrcnieusl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtndjxaevd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtyfmdfoes.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtsvhetxgw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.kuanghao11.cn/gtmyiuvgfu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yj20258.top/gtibteypnj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtwdlrfnxi.html

Q SQL 专题                              90
来源：http://hz.svipenyu.cn/gtshgmzrcm.html

R Bash 专题                             80
来源：http://hz.ybcxt.top/gtfptwzyau.html

S C / C++ 专题                          60
来源：http://hz.yvedp.cn/gtcpiaywig.html

T 其他语言补充                          60
来源：http://hz.ybcxt.top/gtmtyosmvi.html

U 高频实用片段                         120
来源：http://hz.yuxming.cn/gtbeupsblc.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtpbusbjly.html

合计                                  2106 条
来源：http://hz.yueranfly.top/gtxvivlfky.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtyyecgkhe.html

使用提醒
来源：http://hz.chenjidiqi.icu/gtjyxpplpd.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gttgjhzvor.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.meibo888.top/gtyuzyrwlz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shanyushiyangtech.top/gtojewyssc.html


<!-- 参考信息 -->