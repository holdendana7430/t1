代发 wailian999

case class User(name: String, age: Int)
来源：http://hz.jinqigfzy.top/gtyvmyvwxj.html

[T57] Scala：模式匹配
来源：http://hz.aizwys.cn/gtlhtfanvs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhengqikj.top/gtxwgzuvif.html

[T58] Scala：函数定义
来源：http://hz.xingfuxueyuan.xyz/gtrzxklsma.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sweek.top/gtvaxcppaw.html

[T59] Scala：循环
来源：http://hz.zhixingplan.top/gtgglecrjx.html

for (i <- 1 to 10) println(i)
来源：http://hz.wangshuangyany.cn/gtifrcktgf.html

[T60] Scala：折叠
来源：http://hz.bjfxy.top/gtwfaegtau.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnqzz.top/gtuymvuykd.html

================================================================================
来源：http://hz.bjfxy.top/gtuirtnbxl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.iojbl.cn/gtrefbbcos.html

================================================================================
来源：http://hz.tanke756.top/gtrzvvrlxn.html

[U01] Py：创建虚拟环境
来源：http://hz.hammf.cn/gtwneqcgpx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sxryk.cn/gtxeyjbgid.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tian-w.cn/gtmupronyk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yangfankeji.com/gtligudgdz.html

[U03] Py：加载 .env 配置
来源：http://hz.tanke756.top/gthnmlaxil.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jlsjyb.cn/gtapcuietn.html

[U04] Py：变量调试打印
来源：http://hz.yj20258888.top/gtvanpanfl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhijiandao.cn/gtosjrpyxm.html

[U05] Py：列表去重且保序
来源：http://hz.zhixingplan.top/gtpfzyimpb.html

list(dict.fromkeys(arr))
来源：http://hz.gogol.net.cn/gtuuanisgg.html

[U06] Py：合并两个字典
来源：http://hz.jlsjyb.cn/gtxbjowjrp.html

{**a, **b}
来源：http://hz.daria6918.cn/gtunhdcwgv.html

[U07] Py：反转字典键值
来源：http://hz.sufxvd.cn/gtgnmkwoym.html

{v: k for k, v in d.items()}
来源：http://hz.jianghu66.top/gtmbtpgprl.html

[U08] Py：展平二维列表
来源：http://hz.jianghu66.top/gtfiagprlb.html

[y for x in nested for y in x]
来源：http://hz.jinqigfzy.top/gtkskxejqw.html

[U09] Py：字典取最大值的键
来源：http://hz.52xcode.cn/gthwquulez.html

max(d, key=d.get)
来源：http://hz.ivvv.top/gtrfrddkjh.html

[U10] Py：按值排序字典
来源：http://hz.hysaishi.cn/gtgzpvxzsv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xingfuxueyuan.xyz/gtuwdvkgph.html

[U11] Py：生成器表达式
来源：http://hz.jinqigfzy.top/gtlqfiyjgf.html

(x * 2 for x in arr)
来源：http://hz.jyoumei.cn/gtxaiuxtor.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.wangshuangyany.cn/gtloyjaaqh.html

Counter(arr).most_common(3)
来源：http://hz.shanyushiyangtech.top/gtgoudlink.html

[U13] Py：固定长度队列
来源：http://hz.pycfn.com/gthrrpclkz.html

deque(maxlen=10)
来源：http://hz.yvedp.cn/gtkxmrtghj.html

[U14] Py：分组收集到列表
来源：http://hz.ehwqpu.com/gtjnfimzyl.html

defaultdict(list)
来源：http://hz.sweek.top/gteultmzlo.html

[U15] Py：高精度计时
来源：http://hz.jinqigfzy.top/gtfksqwwej.html

t = time.perf_counter()
来源：http://hz.daria6918.cn/gtknwbmdef.html

[U16] Py：命令行参数解析
来源：http://hz.andypj.xyz/gtwkyzyfwd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jyoumei.cn/gtvqprykdg.html

[U17] Py：初始化日志
来源：http://hz.chenlongwang.top/gtaxlezyot.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.daria6918.cn/gtdhjsyjyt.html

[U18] Py：预编译正则
来源：http://hz.yangfankeji.com/gtoauuxxtp.html

pat = re.compile(r"\d+")
来源：http://hz.ehwqpu.com/gtjacyszqm.html

[U19] Py：正则替换带回调
来源：http://hz.havefunace.top/gtunfjbogz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yangfankeji.com/gtdncjalfj.html

[U20] Py：缓存函数结果
来源：http://hz.xingfuxueyuan.xyz/gtkpwfzske.html

@functools.lru_cache(maxsize=None)
来源：http://hz.chenjidiqi.icu/gtnrrctaew.html

[U21] Py：自定义上下文管理器
来源：http://hz.yj202588.top/gtmiktzerr.html

@contextlib.contextmanager
来源：http://hz.shuidangran.top/gtuxsevwjm.html

[U22] Py：矩阵转置
来源：http://hz.aibaodan.cn/gtnzrjmlhv.html

list(zip(*m))
来源：http://hz.shangyingyoupin.top/gtzsmfzotu.html

[U23] Py：分块读取大文件
来源：http://hz.hammf.cn/gtnbpdqhqr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.tian-w.cn/gtxmbcxhec.html

[U24] Py：路径操作
来源：http://hz.yueranfly.top/gtxgskmtrt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gotoacloud.top/gtjopqtvbc.html

[U25] Py：CSV 按字典读
来源：http://hz.chenjidiqi.icu/gtjvxtnhsw.html

csv.DictReader(f)
来源：http://hz.smart0.xyz/gtltkswfll.html

[U26] Py：并发下载
来源：http://hz.nanxuanxn.top/gthnutgcap.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cdnleiting.top/gtuhtvtlkk.html

[U27] Py：异步 HTTP
来源：http://hz.zhiwuduotai.top/gtircfjtxr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xuetiantiany.cn/gtanfwkovk.html

[U28] Py：类型别名
来源：http://hz.wangshuangyany.cn/gttlxnklql.html

UserId = int
来源：http://hz.sxryk.cn/gtpihkqgfs.html

[U29] Py：属性校验
来源：http://hz.smart0.xyz/gthohmaczt.html

@property 与 @x.setter 配合
来源：http://hz.yvedp.cn/gtufhlkjpf.html

[U30] Py：数据类
来源：http://hz.iojbl.cn/gtgozuvhgp.html

@dataclass(slots=True)
来源：http://hz.ydjk.org.cn/gtnhyhmdwa.html

[U31] Py：单测
来源：http://hz.aibaodan.cn/gtpglsnutg.html

python -m pytest -q
来源：http://hz.hnqzz.top/gtkflmcuak.html

[U32] Py：代码格式化
来源：http://hz.ydzc1.top/gtqdnfhmyr.html

ruff format . && ruff check --fix .
来源：http://hz.dashuyun.cn/gtvnjiazos.html

[U33] Py：打包发布
来源：http://hz.0kj1m.cn/gtkjdvhtsn.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jianghu66.top/gtgtynmvbg.html

[U34] Py：判断编码
来源：http://hz.zhaomingkeji.xyz/gtimjkgzrs.html

chardet.detect(raw)
来源：http://hz.tian-w.cn/gtieloqwyg.html

[U35] Py：发送邮件
来源：http://hz.dianchejie.cn/gtdaenlqgb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fzhhl.top/gtbokarbyg.html

[U36] Py：定时任务
来源：http://hz.aibaodan.cn/gtftaqdbyb.html

schedule.every(10).minutes.do(job)
来源：http://hz.xinyue.icu/gtiosunlee.html

[U37] Py：读写 Excel
来源：http://hz.yongpay.top/gtvndorjmm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aizwys.cn/gttpnqxhxo.html

[U38] Py：获取脚本所在目录
来源：http://hz.shanyushiyangkeji.top/gtaopfugho.html

Path(__file__).resolve().parent
来源：http://hz.havefunace.top/gteugaaata.html

[U39] Py：判断是否在交互环境
来源：http://hz.hnxiangtu.top/gtwxxgqtgk.html

sys.stdout.isatty()
来源：http://hz.nanxinkj.top/gtrjoxpthn.html

[U40] Py：打印到标准错误
来源：http://hz.hnxiangtu.top/gtecpxynfe.html

print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtyfvrjihh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.feifeiyinyue.top/gtgnnwmtyl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zdqjudy.top/gtmdcwofcs.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xuanzx.com/gtavpgxwdo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.vqdsnc.cn/gtwtbibpuj.html

[U43] PHP：声明命名空间
来源：http://hz.52xcode.cn/gtgwooosvr.html

namespace App\Http;
来源：http://hz.shanyushiyangtech.top/gtxlquwlld.html

[U44] PHP：开启严格类型
来源：http://hz.9152youxi.cn/gtuwmekddm.html

declare(strict_types=1);
来源：http://hz.316326.xyz/gteedfcjhm.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xuanzx.com/gtlsuztwmw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cheryme.top/gtzslthtqm.html

[U46] PHP：可空类型
来源：http://hz.xuetiantiany.cn/gtvurbtvkd.html

?string $name = null
来源：http://hz.hnxiangtu.top/gtdjkwwvdc.html

[U47] PHP：联合类型
来源：http://hz.yueranfly.top/gtgpwhsbtd.html

int|string $id
来源：http://hz.jinqigfzy.top/gtfduxowky.html

[U48] PHP：纯枚举
来源：http://hz.gotoacloud.top/gtturizkah.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.fengsongda.top/gtirehbytp.html

[U49] PHP：只读属性
来源：http://hz.yongpay.top/gtzwwhacyk.html

public readonly string $name
来源：http://hz.yuxming.cn/gtxyfbdeis.html

[U50] PHP：构造器属性提升
来源：http://hz.tanke756.top/gtqcsdmeuw.html

public function __construct(private int $id) {}
来源：http://hz.0kj1m.cn/gtbtgzfsxb.html

[U51] PHP：数组解构
来源：http://hz.yangfankeji.com/gtcyquzikn.html

[$a, $b] = $arr;
来源：http://hz.daxiang520.top/gtbsnestbf.html

[U52] PHP：箭头函数
来源：http://hz.cucudq.cn/gtvcsqtfbr.html

$double = fn($x) => $x * 2;
来源：http://hz.hfpthk.cn/gtkjknrymp.html

[U53] PHP：空合并运算符
来源：http://hz.yanxiufei.cn/gtzqpbvvvm.html

$v = $a ?? $b ?? "default";
来源：http://hz.zdqjudy.top/gtkakjtygb.html

[U54] PHP：空安全调用
来源：http://hz.dashuyun.cn/gtuhhbgbvp.html

$obj?->method()
来源：http://hz.cdnleiting.top/gtmebiyziz.html

[U55] PHP：match 表达式
来源：http://hz.yanxiufei.cn/gtaibtmgsi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhongyouzk.top/gtfcwdhdlp.html

[U56] PHP：命名参数
来源：http://hz.havefunace.top/gtvvqdgopo.html

f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtoxpraqwo.html

[U57] PHP：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtlhkbhcrs.html

"值: {$a}"
来源：http://hz.aibaodan.cn/gtwldgiqrc.html

[U58] PHP：数组三件套
来源：http://hz.yueranfly.top/gtaslhdasp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.iojbl.cn/gttdotcrsi.html

[U59] PHP：自定义排序
来源：http://hz.aibaodan.cn/gtoecmvdoj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gtxzvhpiyc.html

[U60] PHP：JSON 编解码
来源：http://hz.shzxlz.cn/gtbeluthyy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guowangkeji.top/gtbehoujfz.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gtqotkpxpb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtqtpfawri.html

[U62] PHP：日期对象
来源：http://hz.redwolf501.top/gtvvdsawwa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aibaodan.cn/gtxmxrmxav.html

[U63] PHP：文件读写
来源：http://hz.birdmap.top/gtbnzuziud.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.wangdashe.top/gtjvtktseb.html

[U64] PHP：目录遍历
来源：http://hz.sysykeji.top/gtvpgooacq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.316326.xyz/gtkvlmyjoa.html

[U65] PHP：会话
来源：http://hz.hnxiangtu.top/gtvxkgpgez.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.nanxuanxn.top/gtjxttbyub.html

[U66] PHP：设置 Cookie
来源：http://hz.yonumen.top/gttllbsnwt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xingfuxueyuan.xyz/gtsumwxnsk.html

[U67] PHP：处理文件上传
来源：http://hz.316326.xyz/gtdfgcrprt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xinyue.icu/gtlktlcvjm.html

[U68] PHP：PDO 连接
来源：http://hz.hammf.cn/gtanwvuqch.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jqgfzy.top/gtokjezuww.html

[U69] PHP：PDO 预处理
来源：http://hz.chenzaomai.com/gtvmrtvfvh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hnqzz.top/gtrcqcrfeb.html

[U70] PHP：PDO 事务
来源：http://hz.birdmap.top/gtvcxlixpn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.tianlin.xyz/gtawxycgrd.html

[U71] PHP：抛出异常
来源：http://hz.tian-w.cn/gtsiurldaq.html

throw new RuntimeException("失败", 500);
来源：http://hz.chenlongwang.top/gtdigpswlm.html

[U72] PHP：写错误日志
来源：http://hz.hfpthk.cn/gtelawbueb.html

error_log("失败: " . $e->getMessage());
来源：http://hz.wangdashe.top/gtcrpqjiqb.html

[U73] PHP：读取 ini 配置
来源：http://hz.hysaishi.cn/gtbkaczopk.html

parse_ini_file("config.ini", true)
来源：http://hz.mhx1999.top/gtdkzucgco.html

[U74] PHP：读取环境变量
来源：http://hz.ybcxt.top/gteeflsvnw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.redwolf501.top/gtsjlgniij.html

[U75] PHP：依赖注入
来源：http://hz.guowangkeji.top/gtpioptdtu.html

composer require psr/container
来源：http://hz.yj20258888.top/gttfbzdbtd.html

[U76] PHP：简单路由
来源：http://hz.meibo888.top/gtdecqjtvb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yj202588.top/gtttbbmybq.html

[U77] PHP：模板渲染
来源：http://hz.jinqigufen.top/gttmfimrsv.html

composer require twig/twig
来源：http://hz.ppjwa.cn/gtwgywrmwr.html

[U78] PHP：单元测试
来源：http://hz.zhiwuduotai.top/gtwrdrkswz.html

composer require --dev phpunit/phpunit
来源：http://hz.guannengcc.top/gtqgenxprr.html

[U79] PHP：静态分析
来源：http://hz.dianchejie.cn/gtsddiigrh.html

composer require --dev phpstan/phpstan
来源：http://hz.birdmap.top/gtjckvgmtz.html

[U80] PHP：代码规范修复
来源：http://hz.zhaomingkeji.xyz/gtjagtqqzu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.svipenyu.cn/gtsyhhicrs.html

[U81] JS：初始化项目
来源：http://hz.cqqwz.cn/gtyknpiccg.html

npm init -y;  npm i express
来源：http://hz.zycfv.cn/gtwjhltkzs.html

[U82] JS：package.json 脚本
来源：http://hz.jqgufenzy.top/gtkzalmwco.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hnxiangtu.top/gthrkfewem.html

[U83] JS：ES Module 导入导出
来源：http://hz.aibaodan.cn/gtgicjrpnc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.guowangkeji.top/gtnekbvtkr.html

[U84] JS：CommonJS 写法
来源：http://hz.hammf.cn/gtqesgbtvv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.daria6918.cn/gtvuqgndxh.html

[U85] JS：可选链
来源：http://hz.hongshengwenyu.top/gtghzrftpj.html

a?.b?.c
来源：http://hz.iojbl.cn/gtcmxlvbdx.html

[U86] JS：空值合并
来源：http://hz.zycfv.cn/gtmvxbstvq.html

a ?? b
来源：http://hz.jianghu66.top/gtghfjjcrg.html

[U87] JS：解构默认值
来源：http://hz.wangdashe.top/gtgeofdtkv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shangyingyoupin.top/gtydrhmvbd.html

[U88] JS：对象展开合并
来源：http://hz.wangshuangyany.cn/gtyzaohvgz.html

{ ...a, ...b }
来源：http://hz.ydzc1.top/gtwnwnxqki.html

[U89] JS：数组去重
来源：http://hz.gogol.net.cn/gtahrazape.html

[...new Set(arr)]
来源：http://hz.hfpthk.cn/gtfytqbwch.html

[U90] JS：数字数组排序
来源：http://hz.hysaishi.cn/gtceslzuki.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gthdlcvlxa.html

[U91] JS：对象键值遍历
来源：http://hz.fzhhl.top/gtzzwkphhp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.0kj1m.cn/gtddburfxe.html

[U92] JS：深拷贝
来源：http://hz.jqgufenzy.top/gtihzdoytb.html

structuredClone(obj)
来源：http://hz.haohaochexian.top/gtfegycbxz.html

[U93] JS：模板字符串
来源：http://hz.meibo888.top/gtuaugmrnd.html

`共 ${n} 条`
来源：http://hz.xuanzx.com/gtmelfpnga.html

[U94] JS：箭头函数
来源：http://hz.svipenyu.cn/gttxyysxrl.html

const double = x => x * 2;
来源：http://hz.fzhhl.top/gtkaulabiv.html

[U95] JS：Promise 包装
来源：http://hz.yj202588.top/gtmmpmqyvc.html

new Promise((resolve, reject) => {})
来源：http://hz.ivvv.top/gttovwryjg.html

[U96] JS：async/await 与异常
来源：http://hz.xuanzx.com/gtndndsrcg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtquzrgjzz.html

[U97] JS：并发请求
来源：http://hz.hysaishi.cn/gtkevvqbeb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gttnnbrfof.html

[U98] JS：fetch 带 JSON
来源：http://hz.yj20258888.top/gtodygiyjn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.meibo888.top/gtktaivyln.html

[U99] JS：事件监听
来源：http://hz.yueranfly.top/gtoekfogua.html

el.addEventListener("click", e => {})
来源：http://hz.pycfn.com/gtgxkssxxt.html

[U100] JS：DOM 查询
来源：http://hz.0kj1m.cn/gtecdvgwba.html

document.querySelector(".item")
来源：http://hz.gogol.net.cn/gtqqupojgr.html

[U101] JS：classList 操作
来源：http://hz.zhoulong.xyz/gtjnxzfidc.html

el.classList.toggle("active")
来源：http://hz.xziqi.cn/gtouzsxtal.html

[U102] JS：本地存储
来源：http://hz.0kj1m.cn/gtylmsilkj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.kuanghao11.cn/gtziymdykg.html

[U103] JS：定时器
来源：http://hz.daria6918.cn/gtivmwkprr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhaomingkeji.xyz/gtupquzrul.html

[U104] JS：防抖
来源：http://hz.redwolf501.top/gtzcststlo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtbvmpuvxc.html

[U105] JS：节流
来源：http://hz.yanxiufei.cn/gtigucqyiq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.52xcode.cn/gtpyisrdwb.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gtppmkukpi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxuanxn.top/gturmfvnym.html

[U107] JS：数字千分位
来源：http://hz.snrcjt.cn/gtjtgtytws.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cqqwz.cn/gthsvingsk.html

[U108] JS：随机整数
来源：http://hz.pengpengdd.cyou/gteugrhhgo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.wangdashe.top/gtejfshbzq.html

[U109] JS：数组分组
来源：http://hz.zhiwuduotai.top/gtoelsdvgn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtiojkthaf.html

[U110] JS：数组分块
来源：http://hz.nanxuanxn.top/gtqvtxescr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.andypj.xyz/gtcieewadr.html

[U111] JS：对象转 Map
来源：http://hz.yj202588.top/gtcovylbjx.html

new Map(Object.entries(obj))
来源：http://hz.ppjwa.cn/gtwbgbgyzc.html

[U112] JS：字符串补位
来源：http://hz.pycfn.com/gtscsyibqf.html

"7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtnfozeybw.html

[U113] JS：正则替换全部
来源：http://hz.tanke756.top/gthbcaxvni.html

s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtpxueqgen.html

[U114] JS：JSON 深比较
来源：http://hz.ivvv.top/gtibryxcep.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtzptgtnvb.html

[U115] JS：生成 UUID
来源：http://hz.jqgfzy.top/gtvrfqrybz.html

crypto.randomUUID()
来源：http://hz.bjfxy.top/gtmbxfxjsl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinghuilouyu.cn/gtohigfqrq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.nanxinkj.top/gtjyxmkodq.html

[U117] JS：单元测试
来源：http://hz.iojbl.cn/gtfnzpbkfj.html

npm i -D vitest;  npx vitest
来源：http://hz.tanke756.top/gtsptkvpmy.html

[U118] JS：开发服务器
来源：http://hz.c1oappe.top/gtymhukcon.html

npm i -D vite;  npx vite
来源：http://hz.iojbl.cn/gtzycfjddf.html

[U119] JS：生产构建
来源：http://hz.hongshengwenyu.top/gtwqftcbgm.html

npx vite build
来源：http://hz.sufxvd.cn/gtcetbdpqm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cucudq.cn/gtsiiiedms.html

import.meta.env.VITE_API_URL
来源：http://hz.dianchejie.cn/gtholykrse.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtkuvlhgax.html

统计汇总
来源：http://hz.wangshuangyany.cn/gteaisawbv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttersihyl.html

按语言统计（条）：
来源：http://hz.hfpthk.cn/gtrnbmkyhu.html

Python ......... 252
来源：http://hz.guannengcc.top/gtokuzxmdw.html

PHP ............ 252
来源：http://hz.iojbl.cn/gtzawgwsli.html

JavaScript ..... 252
来源：http://hz.9152youxi.cn/gtzuziijvi.html

TypeScript ..... 212
来源：http://hz.vqdsnc.cn/gtcxdosqvp.html

Java ........... 212
来源：http://hz.shanyushiyangkeji.top/gtmdadxcjk.html

Go ............. 212
来源：http://hz.ybcxt.top/gtuysmbhgr.html

Ruby ........... 212
来源：http://hz.jianghu66.top/gtsaozvitk.html

C# ............. 212
来源：http://hz.ydjk.org.cn/gtbpbztrbr.html

C .............. 30
来源：http://hz.shanyushiyangtech.top/gtwiyukjog.html

C++ ............ 30
来源：http://hz.havefunace.top/gtqrrnkimb.html

SQL ............ 90
来源：http://hz.yvedp.cn/gteiujwfkr.html

Bash ........... 80
来源：http://hz.havefunace.top/gtehmoufii.html

Kotlin ......... 15
来源：http://hz.ppjwa.cn/gtenshlnln.html

Swift .......... 15
来源：http://hz.hongshengwenyu.top/gtbsuqnwlh.html

Lua ............ 10
来源：http://hz.fengsongda.top/gtaitsbadt.html

Perl ........... 10
来源：http://hz.quarkkingdee.top/gtmtaulksy.html

Scala .......... 10
来源：http://hz.smart0.xyz/gtsnujmlfj.html

------------------------------------
来源：http://hz.xuanzx.com/gtelqmaran.html

合计 ........... 2106 条
来源：http://hz.dianchejie.cn/gtmuazjiaq.html

按章节统计：
来源：http://hz.snrcjt.cn/gtghbolmll.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gaohongyu789.top/gtelijdjdi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtedoauuvg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenlongwang.top/gtdjgrybbw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yueranfly.top/gtddukhkjm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.dianchejie.cn/gtsfuskntu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.tanke756.top/gtvbjuyomf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.meibo888.top/gtdxufmldz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtdtkxsqkt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtgtfbigsw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shuidangran.top/gtsplkiuxp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtjvzdmekw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gtozkzaxyu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtwvdwpkea.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.dashuyun.cn/gtdxadplzd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hnxiangtu.top/gtkfrgxgqg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtgretuqhl.html

Q SQL 专题                              90
来源：http://hz.sufxvd.cn/gtjfcysyng.html

R Bash 专题                             80
来源：http://hz.zhoulong.xyz/gtwidnmyae.html

S C / C++ 专题                          60
来源：http://hz.chenjidiqi.icu/gtnspsybge.html

T 其他语言补充                          60
来源：http://hz.dashuyun.cn/gtghmxqrdf.html

U 高频实用片段                         120
来源：http://hz.shangyingyoupin.top/gtpmfhiari.html

------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtoribehnb.html

合计                                  2106 条
来源：http://hz.ppjwa.cn/gtznyrdzvc.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gtemgdwiyr.html


<!-- 参考信息 -->