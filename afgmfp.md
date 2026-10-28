代发 wailian999

[U01] Py：创建虚拟环境
来源：http://hz.ivvv.top/gtuxjixnrk.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cucudq.cn/gtcdrdpvoq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gotoacloud.top/gtkhakehox.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinghuilouyu.cn/gtefqtjlct.html

[U03] Py：加载 .env 配置
来源：http://hz.havefunace.top/gtbhtdtgbs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhengqikj.top/gtdtsxkoyx.html

[U04] Py：变量调试打印
来源：http://hz.cheryme.top/gtlyyttsln.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nanxinkj.top/gtlnzbtjng.html

[U05] Py：列表去重且保序
来源：http://hz.zycfv.cn/gtfwuhhfcy.html

list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtsyrjkopz.html

[U06] Py：合并两个字典
来源：http://hz.jyoumei.cn/gtvlmlwepy.html

{**a, **b}
来源：http://hz.birdmap.top/gtcwjgedcm.html

[U07] Py：反转字典键值
来源：http://hz.andypj.xyz/gtdxnsyqgj.html

{v: k for k, v in d.items()}
来源：http://hz.snrcjt.cn/gttwgtseez.html

[U08] Py：展平二维列表
来源：http://hz.ywan-chungtsiang.top/gtzfbwmhih.html

[y for x in nested for y in x]
来源：http://hz.cashguo.top/gtchbbiays.html

[U09] Py：字典取最大值的键
来源：http://hz.dashuyun.cn/gtnsbabpjv.html

max(d, key=d.get)
来源：http://hz.nanxuanxn.top/gthzipnhdr.html

[U10] Py：按值排序字典
来源：http://hz.andypj.xyz/gtlprsjofz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yanxiufei.cn/gtzvonfpui.html

[U11] Py：生成器表达式
来源：http://hz.yueranfly.top/gtscngkbjm.html

(x * 2 for x in arr)
来源：http://hz.xingfuxueyuan.xyz/gtgjxzsgti.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yonumen.top/gtznuoqeia.html

Counter(arr).most_common(3)
来源：http://hz.aibaodan.cn/gtjfwqbihd.html

[U13] Py：固定长度队列
来源：http://hz.jiagoushi.top/gtxqkfatxv.html

deque(maxlen=10)
来源：http://hz.pengpengdd.cyou/gtneeazkmg.html

[U14] Py：分组收集到列表
来源：http://hz.zhixingplan.top/gtixhhcccq.html

defaultdict(list)
来源：http://hz.hnxiangtu.top/gtmoebosif.html

[U15] Py：高精度计时
来源：http://hz.jinghuilouyu.cn/gtzvpwdcgy.html

t = time.perf_counter()
来源：http://hz.nwbrower.top/gtdvossezd.html

[U16] Py：命令行参数解析
来源：http://hz.ydzc1.top/gtaoumdetj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.fengsongda.top/gtlktkydaq.html

[U17] Py：初始化日志
来源：http://hz.tianlin.xyz/gtaoockmry.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shanyushiyangkeji.top/gtysrsvpnb.html

[U18] Py：预编译正则
来源：http://hz.jinqigufen.top/gtoceeytdt.html

pat = re.compile(r"\d+")
来源：http://hz.quarkkingdee.top/gtbgourzix.html

[U19] Py：正则替换带回调
来源：http://hz.quarkkingdee.top/gttojjymgx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.0kj1m.cn/gtnbuegcju.html

[U20] Py：缓存函数结果
来源：http://hz.jqgfzy.top/gtovetnhoe.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nwbrower.top/gtwnahqgnp.html

[U21] Py：自定义上下文管理器
来源：http://hz.pycfn.com/gtsomzmeyw.html

@contextlib.contextmanager
来源：http://hz.haohaochexian.top/gthlamzhjt.html

[U22] Py：矩阵转置
来源：http://hz.zhongyouzk.top/gtpjuzrmjk.html

list(zip(*m))
来源：http://hz.xziqi.cn/gtxkajhmgi.html

[U23] Py：分块读取大文件
来源：http://hz.gaohongyu789.top/gtjcwqbpgg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sysykeji.top/gtclwqugzl.html

[U24] Py：路径操作
来源：http://hz.cqqwz.cn/gtzjwbqizp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtbcsxyoni.html

[U25] Py：CSV 按字典读
来源：http://hz.redwolf501.top/gtrxpcqpmj.html

csv.DictReader(f)
来源：http://hz.wangdashe.top/gtmzkjsgyj.html

[U26] Py：并发下载
来源：http://hz.gotoacloud.top/gtbslyqgvq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gogol.net.cn/gtigcrziog.html

[U27] Py：异步 HTTP
来源：http://hz.birdmap.top/gtskzgbxwq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.wangdashe.top/gtrtojkmpm.html

[U28] Py：类型别名
来源：http://hz.jqgfzy.top/gtnksbbitg.html

UserId = int
来源：http://hz.xylfe.cn/gtebzrknlt.html

[U29] Py：属性校验
来源：http://hz.jqgufenzy.top/gtnyjjukoq.html

@property 与 @x.setter 配合
来源：http://hz.tianlin.xyz/gtlmldolmv.html

[U30] Py：数据类
来源：http://hz.yuanzhike.top/gtmjfnqgjj.html

@dataclass(slots=True)
来源：http://hz.gotoacloud.top/gtepgqrgnu.html

[U31] Py：单测
来源：http://hz.shuidangran.top/gtxcqvproc.html

python -m pytest -q
来源：http://hz.shanyushiyangtech.top/gtmbzzyols.html

[U32] Py：代码格式化
来源：http://hz.chenzaomai.com/gtdtitvxzx.html

ruff format . && ruff check --fix .
来源：http://hz.jianghu66.top/gtblqoqphv.html

[U33] Py：打包发布
来源：http://hz.shangyingyoupin.top/gtfilrdytq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jyoumei.cn/gtrzlynpct.html

[U34] Py：判断编码
来源：http://hz.cashguo.top/gtoxlboifc.html

chardet.detect(raw)
来源：http://hz.zhengqikj.top/gtqdsrhwnh.html

[U35] Py：发送邮件
来源：http://hz.xylfe.cn/gtrthucnrs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zdqjudy.top/gtdfokheay.html

[U36] Py：定时任务
来源：http://hz.shzxlz.cn/gtzfuseifs.html

schedule.every(10).minutes.do(job)
来源：http://hz.haohaochexian.top/gtvaqnukdd.html

[U37] Py：读写 Excel
来源：http://hz.yj20258.top/gtmomfeyeb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hywenlv.cn/gtnradiafj.html

[U38] Py：获取脚本所在目录
来源：http://hz.fengsongda.top/gtdhyojvaa.html

Path(__file__).resolve().parent
来源：http://hz.pycfn.com/gtgtrnvzur.html

[U39] Py：判断是否在交互环境
来源：http://hz.zycfv.cn/gtkxhrulro.html

sys.stdout.isatty()
来源：http://hz.nanxuanxn.top/gttmahbvpb.html

[U40] Py：打印到标准错误
来源：http://hz.yuanzhike.top/gtnlzlhkfz.html

print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtsfqgrcgr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.iojbl.cn/gtylbuaosx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cheryme.top/gtbfybqjml.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.mhx1999.top/gtspdbqbhb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gotoacloud.top/gtlzfeblth.html

[U43] PHP：声明命名空间
来源：http://hz.hammf.cn/gthjjieoih.html

namespace App\Http;
来源：http://hz.zhaomingkeji.xyz/gtxlqjxouz.html

[U44] PHP：开启严格类型
来源：http://hz.ppjwa.cn/gtwezwnymw.html

declare(strict_types=1);
来源：http://hz.tanke756.top/gtkxnbhekk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.c1oappe.top/gtildbzyhw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtnvcttnwt.html

[U46] PHP：可空类型
来源：http://hz.tanke756.top/gthzpepbsd.html

?string $name = null
来源：http://hz.daxiang520.top/gtjdcieqib.html

[U47] PHP：联合类型
来源：http://hz.iojbl.cn/gthfypxbff.html

int|string $id
来源：http://hz.daria6918.cn/gtizkeaxao.html

[U48] PHP：纯枚举
来源：http://hz.iojbl.cn/gtjgamgede.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shzxlz.cn/gtzvrlymsa.html

[U49] PHP：只读属性
来源：http://hz.hysaishi.cn/gtdslwjcvw.html

public readonly string $name
来源：http://hz.nanxinkj.top/gtcrequdgz.html

[U50] PHP：构造器属性提升
来源：http://hz.aibaodan.cn/gtitqjgusn.html

public function __construct(private int $id) {}
来源：http://hz.wangdashe.top/gtqahyudya.html

[U51] PHP：数组解构
来源：http://hz.gaohongyu789.top/gtxehvkdsk.html

[$a, $b] = $arr;
来源：http://hz.fengsongda.top/gtflhfkasm.html

[U52] PHP：箭头函数
来源：http://hz.jqgfzy.top/gtztzytijk.html

$double = fn($x) => $x * 2;
来源：http://hz.shuidangran.top/gtenqcjoip.html

[U53] PHP：空合并运算符
来源：http://hz.ppjwa.cn/gtklnqrfoq.html

$v = $a ?? $b ?? "default";
来源：http://hz.haohaochexian.top/gtwpizzxcr.html

[U54] PHP：空安全调用
来源：http://hz.shanyushiyangkeji.top/gtpfvpwdzq.html

$obj?->method()
来源：http://hz.daria6918.cn/gtyxrulqnj.html

[U55] PHP：match 表达式
来源：http://hz.xinyue.icu/gtlqjbvrlf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.havefunace.top/gttfbzdcei.html

[U56] PHP：命名参数
来源：http://hz.xuanzx.com/gtktmfpupl.html

f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtmayjqxcv.html

[U57] PHP：字符串插值
来源：http://hz.wangshuangyany.cn/gtrckqoous.html

"值: {$a}"
来源：http://hz.xinyue.icu/gtozuvqopo.html

[U58] PHP：数组三件套
来源：http://hz.cheryme.top/gtzzbbepqg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.haohaochexian.top/gtayokchcv.html

[U59] PHP：自定义排序
来源：http://hz.ydzc1.top/gtazqykfsk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.52xcode.cn/gtaqwyuail.html

[U60] PHP：JSON 编解码
来源：http://hz.chenzaomai.com/gtyghclfib.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ivvv.top/gtilgxrbsc.html

[U61] PHP：正则
来源：http://hz.sweek.top/gtfrgtffce.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtkohzcwww.html

[U62] PHP：日期对象
来源：http://hz.dashuyun.cn/gtpdlizrqj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhongyouzk.top/gtumdkhdeh.html

[U63] PHP：文件读写
来源：http://hz.zhaomingkeji.xyz/gtdsvyidpz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sufxvd.cn/gtdrlylcga.html

[U64] PHP：目录遍历
来源：http://hz.yj20258888.top/gtuesdjokt.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sweek.top/gtmjhdyfjt.html

[U65] PHP：会话
来源：http://hz.gotoacloud.top/gtdixwyzwz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jqgufenzy.top/gthzckdihb.html

[U66] PHP：设置 Cookie
来源：http://hz.ivvv.top/gtthgjaegy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cdnleiting.top/gtkcwkqjcc.html

[U67] PHP：处理文件上传
来源：http://hz.tianlin.xyz/gtbreygiln.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yueranfly.top/gtsmgpalqs.html

[U68] PHP：PDO 连接
来源：http://hz.vqdsnc.cn/gtkiripvuy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jqgufenzy.top/gtwkzabuxo.html

[U69] PHP：PDO 预处理
来源：http://hz.nanxuanxn.top/gtvsxklzhw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.haohaochexian.top/gtjwwacqxq.html

[U70] PHP：PDO 事务
来源：http://hz.vqdsnc.cn/gtebwbfwyb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhongyouzk.top/gtiaeaviyj.html

[U71] PHP：抛出异常
来源：http://hz.zycfv.cn/gtupvetdto.html

throw new RuntimeException("失败", 500);
来源：http://hz.xylfe.cn/gtlhypuwtz.html

[U72] PHP：写错误日志
来源：http://hz.birdmap.top/gtsjnixibo.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yongpay.top/gtwikadtii.html

[U73] PHP：读取 ini 配置
来源：http://hz.316326.xyz/gtnpbjhkdf.html

parse_ini_file("config.ini", true)
来源：http://hz.cucudq.cn/gtwhvcstzk.html

[U74] PHP：读取环境变量
来源：http://hz.hywenlv.cn/gtsysrwuuy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gaohongyu789.top/gtvpbsprpe.html

[U75] PHP：依赖注入
来源：http://hz.0kj1m.cn/gtncplcneh.html

composer require psr/container
来源：http://hz.svipenyu.cn/gtptnhbstv.html

[U76] PHP：简单路由
来源：http://hz.yongpay.top/gtnuzleoic.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yj20258888.top/gtrpdfhzci.html

[U77] PHP：模板渲染
来源：http://hz.chenlongwang.top/gtcbfdeoju.html

composer require twig/twig
来源：http://hz.xuanzx.com/gtjlasneyq.html

[U78] PHP：单元测试
来源：http://hz.yvedp.cn/gtqerwmzhq.html

composer require --dev phpunit/phpunit
来源：http://hz.9152youxi.cn/gtcejtehqo.html

[U79] PHP：静态分析
来源：http://hz.jyoumei.cn/gtbivugckf.html

composer require --dev phpstan/phpstan
来源：http://hz.hnqzz.top/gtsqpcawia.html

[U80] PHP：代码规范修复
来源：http://hz.shzxlz.cn/gtjxaxbtnq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ybcxt.top/gtkyixrspe.html

[U81] JS：初始化项目
来源：http://hz.yongpay.top/gtglywyjxw.html

npm init -y;  npm i express
来源：http://hz.dashuyun.cn/gtsrippigx.html

[U82] JS：package.json 脚本
来源：http://hz.feifeiyinyue.top/gttspvulxu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinghuilouyu.cn/gtjaxafbld.html

[U83] JS：ES Module 导入导出
来源：http://hz.hammf.cn/gtjbrknlal.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.0kj1m.cn/gthaekjdvh.html

[U84] JS：CommonJS 写法
来源：http://hz.yvedp.cn/gtidfcbuvn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.dianchejie.cn/gtekmoymbi.html

[U85] JS：可选链
来源：http://hz.xylfe.cn/gtjcmwrzwp.html

a?.b?.c
来源：http://hz.shzxlz.cn/gtudwvdumf.html

[U86] JS：空值合并
来源：http://hz.ydjk.org.cn/gtmiuurwpk.html

a ?? b
来源：http://hz.jinyuanbaomall.cn/gtmkmycdbh.html

[U87] JS：解构默认值
来源：http://hz.jyoumei.cn/gtqmzeazjr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.snrcjt.cn/gtqxaqjmiz.html

[U88] JS：对象展开合并
来源：http://hz.quarkkingdee.top/gttizwdxhk.html

{ ...a, ...b }
来源：http://hz.aibaodan.cn/gtxsoqesvc.html

[U89] JS：数组去重
来源：http://hz.aizwys.cn/gtqgdhtuiy.html

[...new Set(arr)]
来源：http://hz.yvedp.cn/gtqcgjgkeq.html

[U90] JS：数字数组排序
来源：http://hz.dashuyun.cn/gtdxlptusr.html

[...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtlxqtbxmh.html

[U91] JS：对象键值遍历
来源：http://hz.zdqjudy.top/gtcdevtwvs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.guowangkeji.top/gtofdtpedj.html

[U92] JS：深拷贝
来源：http://hz.316326.xyz/gtmdafofuk.html

structuredClone(obj)
来源：http://hz.meibo888.top/gtpjwtbtbz.html

[U93] JS：模板字符串
来源：http://hz.jinqigufen.top/gtufiywkyd.html

`共 ${n} 条`
来源：http://hz.xuanzx.com/gthczwwyeg.html

[U94] JS：箭头函数
来源：http://hz.0kj1m.cn/gtgoelgeaf.html

const double = x => x * 2;
来源：http://hz.52xcode.cn/gtmtpohnyu.html

[U95] JS：Promise 包装
来源：http://hz.iojbl.cn/gtasppaayn.html

new Promise((resolve, reject) => {})
来源：http://hz.yangfankeji.com/gticnuuomg.html

[U96] JS：async/await 与异常
来源：http://hz.cashguo.top/gtkhjbpqwp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtyjsgecnp.html

[U97] JS：并发请求
来源：http://hz.hfpthk.cn/gtzklpkrzn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtedswbngv.html

[U98] JS：fetch 带 JSON
来源：http://hz.xinyue.icu/gthsjaxmxm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhongyouzk.top/gtmylgedhc.html

[U99] JS：事件监听
来源：http://hz.xuetiantiany.cn/gtvwllajga.html

el.addEventListener("click", e => {})
来源：http://hz.ehwqpu.com/gtfqorpqoo.html

[U100] JS：DOM 查询
来源：http://hz.yueranfly.top/gtbcagqivx.html

document.querySelector(".item")
来源：http://hz.9152youxi.cn/gtdigrspme.html

[U101] JS：classList 操作
来源：http://hz.zhongyouzk.top/gtzmqfxpjn.html

el.classList.toggle("active")
来源：http://hz.xuetiantiany.cn/gtjeduvrsp.html

[U102] JS：本地存储
来源：http://hz.dashuyun.cn/gtujzmczqe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zycfv.cn/gthimrfnxe.html

[U103] JS：定时器
来源：http://hz.xingfuxueyuan.xyz/gtzxlqwowf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guannengcc.top/gtdtmpyhws.html

[U104] JS：防抖
来源：http://hz.ybcxt.top/gtajbvwwud.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtgzspyfqo.html

[U105] JS：节流
来源：http://hz.gogol.net.cn/gttjdcbnen.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenlongwang.top/gtofxdmbpd.html

[U106] JS：日期格式化
来源：http://hz.yongpay.top/gtgzzoogfq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhoulong.xyz/gtyjgpyywo.html

[U107] JS：数字千分位
来源：http://hz.cqqwz.cn/gtgueggfkw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jqgufenzy.top/gtpskjgxbw.html

[U108] JS：随机整数
来源：http://hz.feifeiyinyue.top/gtmuiwqwer.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ivvv.top/gtcldlectr.html

[U109] JS：数组分组
来源：http://hz.daxiang520.top/gttevsgxsp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtbzpwhfit.html

[U110] JS：数组分块
来源：http://hz.yvedp.cn/gtdnbigpep.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sxryk.cn/gtcqiyukjt.html

[U111] JS：对象转 Map
来源：http://hz.zdqjudy.top/gtgckxzpba.html

new Map(Object.entries(obj))
来源：http://hz.birdmap.top/gtbchculmz.html

[U112] JS：字符串补位
来源：http://hz.jinghuilouyu.cn/gtrgtwmmos.html

"7".padStart(3, "0")
来源：http://hz.jianghu66.top/gttxyerdvp.html

[U113] JS：正则替换全部
来源：http://hz.shzxlz.cn/gtziyinyov.html

s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtgedmnofu.html

[U114] JS：JSON 深比较
来源：http://hz.aizwys.cn/gtwinrxxdb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gtzphrwipu.html

[U115] JS：生成 UUID
来源：http://hz.mhx1999.top/gtqjmdxprv.html

crypto.randomUUID()
来源：http://hz.ivvv.top/gtrslfjxim.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yangfankeji.com/gtohwovkpl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sufxvd.cn/gtaccrtitt.html

[U117] JS：单元测试
来源：http://hz.jlsjyb.cn/gtyrlqttkj.html

npm i -D vitest;  npx vitest
来源：http://hz.tianlin.xyz/gtgwtfpldf.html

[U118] JS：开发服务器
来源：http://hz.yanxiufei.cn/gttzyrilku.html

npm i -D vite;  npx vite
来源：http://hz.hnxiangtu.top/gtcjezaamk.html

[U119] JS：生产构建
来源：http://hz.ppjwa.cn/gthakgqpvj.html

npx vite build
来源：http://hz.ybcxt.top/gtidbhsviy.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yueranfly.top/gtiezaynny.html

import.meta.env.VITE_API_URL
来源：http://hz.jinqigufen.top/gtqvslsdoe.html

================================================================================
来源：http://hz.316326.xyz/gtrtcqrpzr.html

统计汇总
来源：http://hz.xuetiantiany.cn/gtkmpgbrln.html

================================================================================
来源：http://hz.dashuyun.cn/gttmfgijrl.html

按语言统计（条）：
来源：http://hz.cheryme.top/gttcnjbcsz.html

Python ......... 252
来源：http://hz.hongshengwenyu.top/gtguspctpt.html

PHP ............ 252
来源：http://hz.pengpengdd.cyou/gtoifabmfh.html

JavaScript ..... 252
来源：http://hz.zhongyouzk.top/gtqmytfglp.html

TypeScript ..... 212
来源：http://hz.havefunace.top/gtqaezxvww.html

Java ........... 212
来源：http://hz.yangfankeji.com/gtcagaqxrn.html

Go ............. 212
来源：http://hz.ybcxt.top/gtidcmeteq.html

Ruby ........... 212
来源：http://hz.hnxiangtu.top/gtkpzmqqne.html

C# ............. 212
来源：http://hz.zhongyouzk.top/gtsijeikgp.html

C .............. 30
来源：http://hz.tanke756.top/gtywpfxysq.html

C++ ............ 30
来源：http://hz.feifeiyinyue.top/gtcaezvdap.html

SQL ............ 90
来源：http://hz.316326.xyz/gteuzihivo.html

Bash ........... 80
来源：http://hz.daxiang520.top/gtksimtqio.html

Kotlin ......... 15
来源：http://hz.xuetiantiany.cn/gtavpahbth.html

Swift .......... 15
来源：http://hz.gotoacloud.top/gtuxzpfvmq.html

Lua ............ 10
来源：http://hz.yanxiufei.cn/gtlhrlvadp.html

Perl ........... 10
来源：http://hz.tanke756.top/gtfndbrlpw.html

Scala .......... 10
来源：http://hz.yvedp.cn/gtmyavlplz.html

------------------------------------
来源：http://hz.ybcxt.top/gtacjzlgyy.html

合计 ........... 2106 条
来源：http://hz.hnqzz.top/gtermnrirh.html

按章节统计：
来源：http://hz.iojbl.cn/gtiagiujkh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhoulong.xyz/gtodehgtge.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ydjk.org.cn/gtyfzeviwl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtpcfmpzif.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtfhjwlpdr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.wangshuangyany.cn/gtppnwqkes.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yj202588.top/gtjnguwack.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtedwrzcbx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sysykeji.top/gtlegctbwf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtchelpcwx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gteoqwjiea.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtufdgnndn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtxzbdwobh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtftcjbysr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sysykeji.top/gtasjfauba.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jqgfzy.top/gtbbylpksc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtcnavzutb.html

Q SQL 专题                              90
来源：http://hz.sweek.top/gtajrjfghi.html

R Bash 专题                             80
来源：http://hz.hywenlv.cn/gtqzmdjvku.html

S C / C++ 专题                          60
来源：http://hz.xziqi.cn/gtcmcingot.html

T 其他语言补充                          60
来源：http://hz.shuidangran.top/gtlxutrelx.html

U 高频实用片段                         120
来源：http://hz.c1oappe.top/gtwxqmmodc.html

------------------------------------
来源：http://hz.tianlin.xyz/gtszyfgyoh.html

合计                                  2106 条
来源：http://hz.chenjidiqi.icu/gtjvyqfmfl.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtlzciejbv.html

使用提醒
来源：http://hz.yuanzhike.top/gtxazgowqa.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtdpjxnhgy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.316326.xyz/gtjktlrcrp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.meibo888.top/gtjwsezvqg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cashguo.top/gtgmkhsden.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yueranfly.top/gtlrrdxdhx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ehwqpu.com/gtfvgqlfny.html

—— 文件结束 ——
来源：http://hz.ybcxt.top/gtditgbqxl.html

================================================================================
来源：http://hz.tianlin.xyz/gtouqolxut.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.vqdsnc.cn/gtlsznthpr.html

Common Programming Examples Cheat Book
来源：http://hz.yj202588.top/gtvwrrxair.html

================================================================================
来源：http://hz.hammf.cn/gtzbsceywo.html


<!-- 参考信息 -->