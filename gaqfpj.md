代发 wailian999

case class User(name: String, age: Int)
来源：http://hz.nwbrower.top/gthrykafis.html

[T57] Scala：模式匹配
来源：http://hz.316326.xyz/gtxdvyzcgx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.9152youxi.cn/gtaivbgknm.html

[T58] Scala：函数定义
来源：http://hz.yj202588.top/gtbkycmayl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhixingplan.top/gtcbafifbo.html

[T59] Scala：循环
来源：http://hz.c1oappe.top/gtlznfauen.html

for (i <- 1 to 10) println(i)
来源：http://hz.jianghu66.top/gtgnprlwku.html

[T60] Scala：折叠
来源：http://hz.ydzc1.top/gtfzawghlc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.meibo888.top/gtnxjyigku.html

================================================================================
来源：http://hz.zhengqikj.top/gtrlieebvr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtwubkachf.html

================================================================================
来源：http://hz.snrcjt.cn/gtxhoofkph.html

[U01] Py：创建虚拟环境
来源：http://hz.tian-w.cn/gtgnfpbnik.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.0kj1m.cn/gtahqobusp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shangyingyoupin.top/gtbqhjffpz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yongpay.top/gtpddhsrin.html

[U03] Py：加载 .env 配置
来源：http://hz.guowangkeji.top/gtgtollmpo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydzc1.top/gtvjwxigcn.html

[U04] Py：变量调试打印
来源：http://hz.xinyue.icu/gtdgvbnryj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.svipenyu.cn/gtjgytidsz.html

[U05] Py：列表去重且保序
来源：http://hz.jiagoushi.top/gtszsylrpn.html

list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gtwwklnfod.html

[U06] Py：合并两个字典
来源：http://hz.yj202588.top/gtxdioukbw.html

{**a, **b}
来源：http://hz.sxryk.cn/gtqujlobgf.html

[U07] Py：反转字典键值
来源：http://hz.zhijiandao.cn/gtllgyvhqd.html

{v: k for k, v in d.items()}
来源：http://hz.xuetiantiany.cn/gtvmnbldbq.html

[U08] Py：展平二维列表
来源：http://hz.xziqi.cn/gtfwscqtee.html

[y for x in nested for y in x]
来源：http://hz.zhaomingkeji.xyz/gtfagcvrgv.html

[U09] Py：字典取最大值的键
来源：http://hz.meibo888.top/gtkjxtaylo.html

max(d, key=d.get)
来源：http://hz.tanke756.top/gtjgukekqm.html

[U10] Py：按值排序字典
来源：http://hz.dianchejie.cn/gtfseoerrv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gaohongyu789.top/gtgmdfirmj.html

[U11] Py：生成器表达式
来源：http://hz.hywenlv.cn/gtehypqmpx.html

(x * 2 for x in arr)
来源：http://hz.aizwys.cn/gtacrqbghb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.dianchejie.cn/gtlkcgthgg.html

Counter(arr).most_common(3)
来源：http://hz.pycfn.com/gtlvpuevru.html

[U13] Py：固定长度队列
来源：http://hz.cashguo.top/gtmbvbyryh.html

deque(maxlen=10)
来源：http://hz.ywan-chungtsiang.top/gtpeogewxi.html

[U14] Py：分组收集到列表
来源：http://hz.havefunace.top/gtxnubkefr.html

defaultdict(list)
来源：http://hz.yvedp.cn/gthxrwdiac.html

[U15] Py：高精度计时
来源：http://hz.zhengqikj.top/gtupupjtop.html

t = time.perf_counter()
来源：http://hz.daxiang520.top/gtgbhpikzd.html

[U16] Py：命令行参数解析
来源：http://hz.hnqzz.top/gthawgspum.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhoulong.xyz/gtwsbspocp.html

[U17] Py：初始化日志
来源：http://hz.9152youxi.cn/gtvtokpjce.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yanxiufei.cn/gtmqtqifik.html

[U18] Py：预编译正则
来源：http://hz.sxryk.cn/gtdlgrkhsg.html

pat = re.compile(r"\d+")
来源：http://hz.wangshuangyany.cn/gtiilcgoup.html

[U19] Py：正则替换带回调
来源：http://hz.bjfxy.top/gtyocqlsyl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhixingplan.top/gtngzdoldt.html

[U20] Py：缓存函数结果
来源：http://hz.jlsjyb.cn/gtuiunnvzj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.redwolf501.top/gtmdhiobtn.html

[U21] Py：自定义上下文管理器
来源：http://hz.xuanzx.com/gtfewhaclc.html

@contextlib.contextmanager
来源：http://hz.chenjidiqi.icu/gtbvprssop.html

[U22] Py：矩阵转置
来源：http://hz.ydjk.org.cn/gtaoqnpcfd.html

list(zip(*m))
来源：http://hz.ybcxt.top/gtmpntvwlh.html

[U23] Py：分块读取大文件
来源：http://hz.andypj.xyz/gtsieubupy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pengpengdd.cyou/gtzdymuxbh.html

[U24] Py：路径操作
来源：http://hz.nwbrower.top/gtejgadrsd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangdashe.top/gtttthausn.html

[U25] Py：CSV 按字典读
来源：http://hz.pycfn.com/gtfctcetsh.html

csv.DictReader(f)
来源：http://hz.hywenlv.cn/gtkhxgczmr.html

[U26] Py：并发下载
来源：http://hz.redwolf501.top/gtsqkkuxdq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.haohaochexian.top/gtxcovxjhk.html

[U27] Py：异步 HTTP
来源：http://hz.cqqwz.cn/gtpkfnxuqk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.quarkkingdee.top/gtxigwixft.html

[U28] Py：类型别名
来源：http://hz.ppjwa.cn/gtbaquzxhl.html

UserId = int
来源：http://hz.0kj1m.cn/gtqyqbtzlo.html

[U29] Py：属性校验
来源：http://hz.yuxming.cn/gtqgpzyqpb.html

@property 与 @x.setter 配合
来源：http://hz.c1oappe.top/gtgwsgaabs.html

[U30] Py：数据类
来源：http://hz.shzxlz.cn/gtwjhubpoo.html

@dataclass(slots=True)
来源：http://hz.birdmap.top/gthcgqtobg.html

[U31] Py：单测
来源：http://hz.havefunace.top/gttixywiyy.html

python -m pytest -q
来源：http://hz.hysaishi.cn/gtggdghrjs.html

[U32] Py：代码格式化
来源：http://hz.jlsjyb.cn/gtqvgdciez.html

ruff format . && ruff check --fix .
来源：http://hz.wangshuangyany.cn/gtncyrbbnv.html

[U33] Py：打包发布
来源：http://hz.gotoacloud.top/gtvjncfsxz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yueranfly.top/gtgseqdpia.html

[U34] Py：判断编码
来源：http://hz.xuanzx.com/gtgpstvrnp.html

chardet.detect(raw)
来源：http://hz.chenzaomai.com/gteqqkbggr.html

[U35] Py：发送邮件
来源：http://hz.jyoumei.cn/gtoxkujnss.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xinyue.icu/gtniavultc.html

[U36] Py：定时任务
来源：http://hz.sweek.top/gtbgacdejo.html

schedule.every(10).minutes.do(job)
来源：http://hz.iojbl.cn/gtfbiuconh.html

[U37] Py：读写 Excel
来源：http://hz.shanyushiyangtech.top/gtqnulczqy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.feifeiyinyue.top/gtndyzgjms.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxuanxn.top/gthtspzwhs.html

Path(__file__).resolve().parent
来源：http://hz.shuidangran.top/gtpivazrrs.html

[U39] Py：判断是否在交互环境
来源：http://hz.sufxvd.cn/gttwxaxvyv.html

sys.stdout.isatty()
来源：http://hz.jinqigufen.top/gttojavzzn.html

[U40] Py：打印到标准错误
来源：http://hz.gzhubu.top/gtljqltxaz.html

print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtqgvldtuf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenlongwang.top/gtybipeozh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.guowangkeji.top/gtzmhfpccu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gotoacloud.top/gtxbafikmm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hysaishi.cn/gtqyqkadhf.html

[U43] PHP：声明命名空间
来源：http://hz.yuanzhike.top/gtirjhzchm.html

namespace App\Http;
来源：http://hz.sysykeji.top/gtqrnhglom.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtblnjatqa.html

declare(strict_types=1);
来源：http://hz.yj20258.top/gtovdzvrmv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hnqzz.top/gtvojvsqmy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtxopoyegg.html

[U46] PHP：可空类型
来源：http://hz.shuidangran.top/gtpurlrqgh.html

?string $name = null
来源：http://hz.0kj1m.cn/gtqhhossjt.html

[U47] PHP：联合类型
来源：http://hz.guowangkeji.top/gttcfzergg.html

int|string $id
来源：http://hz.jqgufenzy.top/gtbrldkvvk.html

[U48] PHP：纯枚举
来源：http://hz.hongshengwenyu.top/gtitqfmvdu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xingfuxueyuan.xyz/gttdeibjap.html

[U49] PHP：只读属性
来源：http://hz.shangyingyoupin.top/gtospcyxxm.html

public readonly string $name
来源：http://hz.smart0.xyz/gtsqlkhzdc.html

[U50] PHP：构造器属性提升
来源：http://hz.xziqi.cn/gthnmzmsnf.html

public function __construct(private int $id) {}
来源：http://hz.jqgfzy.top/gtnbzavlqf.html

[U51] PHP：数组解构
来源：http://hz.52xcode.cn/gthegmylip.html

[$a, $b] = $arr;
来源：http://hz.jinghuilouyu.cn/gtgicedxtb.html

[U52] PHP：箭头函数
来源：http://hz.shanyushiyangtech.top/gtocrsepka.html

$double = fn($x) => $x * 2;
来源：http://hz.xingfuxueyuan.xyz/gtwxfkvpgq.html

[U53] PHP：空合并运算符
来源：http://hz.cashguo.top/gtucattjdq.html

$v = $a ?? $b ?? "default";
来源：http://hz.xziqi.cn/gtjdirwnnq.html

[U54] PHP：空安全调用
来源：http://hz.yuanzhike.top/gtlkzzujop.html

$obj?->method()
来源：http://hz.ppjwa.cn/gtmxuypioz.html

[U55] PHP：match 表达式
来源：http://hz.hfpthk.cn/gtoiahfddi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.smart0.xyz/gtbbddqhib.html

[U56] PHP：命名参数
来源：http://hz.cqqwz.cn/gtwzfcdqpp.html

f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtlmvugigs.html

[U57] PHP：字符串插值
来源：http://hz.quarkkingdee.top/gtjpvphydb.html

"值: {$a}"
来源：http://hz.zhijiandao.cn/gthuidcbtu.html

[U58] PHP：数组三件套
来源：http://hz.guowangkeji.top/gtlqrxosuu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.smart0.xyz/gtkyywosxt.html

[U59] PHP：自定义排序
来源：http://hz.chenzaomai.com/gtbxybeeia.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shzxlz.cn/gtbwvqznok.html

[U60] PHP：JSON 编解码
来源：http://hz.hammf.cn/gtyxotxwag.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258888.top/gtyvavwzms.html

[U61] PHP：正则
来源：http://hz.xingfuxueyuan.xyz/gtfvqdxikx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuetiantiany.cn/gtfoolocof.html

[U62] PHP：日期对象
来源：http://hz.jqgufenzy.top/gtupxpofoh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shanyushiyangtech.top/gtyiqelpqr.html

[U63] PHP：文件读写
来源：http://hz.zhixingplan.top/gtnkmnlhoz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenjidiqi.icu/gtlcjqqbai.html

[U64] PHP：目录遍历
来源：http://hz.jqgfzy.top/gtoliqkwoy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hysaishi.cn/gtzvklvadq.html

[U65] PHP：会话
来源：http://hz.zhiwuduotai.top/gtugkeyndh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jqgufenzy.top/gtvynyuvzf.html

[U66] PHP：设置 Cookie
来源：http://hz.xingfuxueyuan.xyz/gtdrxpmhnf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yangfankeji.com/gthrnqiwdf.html

[U67] PHP：处理文件上传
来源：http://hz.dashuyun.cn/gteokznknq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cdnleiting.top/gtczzvbcig.html

[U68] PHP：PDO 连接
来源：http://hz.c1oappe.top/gtllmmyenw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cdnleiting.top/gtvqmdscan.html

[U69] PHP：PDO 预处理
来源：http://hz.gogol.net.cn/gtdbapakqs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cucudq.cn/gtqwjdcpov.html

[U70] PHP：PDO 事务
来源：http://hz.nanxuanxn.top/gtqrbmxybx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ydzc1.top/gtpvtdvvwd.html

[U71] PHP：抛出异常
来源：http://hz.xziqi.cn/gtrcywgumx.html

throw new RuntimeException("失败", 500);
来源：http://hz.nanxuanxn.top/gtvkmqwpkf.html

[U72] PHP：写错误日志
来源：http://hz.sxryk.cn/gtkdewbmoe.html

error_log("失败: " . $e->getMessage());
来源：http://hz.haohaochexian.top/gtmksptyos.html

[U73] PHP：读取 ini 配置
来源：http://hz.hnxiangtu.top/gtulnqjxrh.html

parse_ini_file("config.ini", true)
来源：http://hz.xylfe.cn/gtvmuohyby.html

[U74] PHP：读取环境变量
来源：http://hz.smart0.xyz/gtvyzoyxdh.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jyoumei.cn/gtathvokhm.html

[U75] PHP：依赖注入
来源：http://hz.52xcode.cn/gtsxvgphyn.html

composer require psr/container
来源：http://hz.tian-w.cn/gtejpfmenk.html

[U76] PHP：简单路由
来源：http://hz.52xcode.cn/gtdxusuzra.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.sysykeji.top/gtqrnvjide.html

[U77] PHP：模板渲染
来源：http://hz.shzxlz.cn/gtgrphfgpa.html

composer require twig/twig
来源：http://hz.ydjk.org.cn/gtlzrjsuml.html

[U78] PHP：单元测试
来源：http://hz.jinqigfzy.top/gtdnebolxr.html

composer require --dev phpunit/phpunit
来源：http://hz.fengsongda.top/gtivcduyow.html

[U79] PHP：静态分析
来源：http://hz.snrcjt.cn/gtqatdwirr.html

composer require --dev phpstan/phpstan
来源：http://hz.zhijiandao.cn/gtiugymaad.html

[U80] PHP：代码规范修复
来源：http://hz.fzhhl.top/gtuoxzalmj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hywenlv.cn/gtxpxtxzmg.html

[U81] JS：初始化项目
来源：http://hz.kuanghao11.cn/gtztckssyb.html

npm init -y;  npm i express
来源：http://hz.pengpengdd.cyou/gtcrvdgmtd.html

[U82] JS：package.json 脚本
来源：http://hz.pengpengdd.cyou/gtlydvheli.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zdqjudy.top/gtkbgwbqgu.html

[U83] JS：ES Module 导入导出
来源：http://hz.yanxiufei.cn/gtveayitcm.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj202588.top/gthvptcvwk.html

[U84] JS：CommonJS 写法
来源：http://hz.fengsongda.top/gtuugfdlvc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinqigfzy.top/gtsbeijbqn.html

[U85] JS：可选链
来源：http://hz.fzhhl.top/gtalitcmps.html

a?.b?.c
来源：http://hz.yangfankeji.com/gtckwvzomw.html

[U86] JS：空值合并
来源：http://hz.zdqjudy.top/gtbytsyssd.html

a ?? b
来源：http://hz.meibo888.top/gtbrssgzmu.html

[U87] JS：解构默认值
来源：http://hz.quarkkingdee.top/gtwxdhoonn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ivvv.top/gtxwkpaiey.html

[U88] JS：对象展开合并
来源：http://hz.cqqwz.cn/gtcdesnbqx.html

{ ...a, ...b }
来源：http://hz.yanxiufei.cn/gtvxdfjugt.html

[U89] JS：数组去重
来源：http://hz.cdnleiting.top/gtlnadidhi.html

[...new Set(arr)]
来源：http://hz.aizwys.cn/gtmieteahi.html

[U90] JS：数字数组排序
来源：http://hz.jianghu66.top/gtrknuetik.html

[...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtpekmajwm.html

[U91] JS：对象键值遍历
来源：http://hz.yj20258.top/gtghoarxiq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ybcxt.top/gtacjmjblk.html

[U92] JS：深拷贝
来源：http://hz.zhengqikj.top/gthsnqxzkx.html

structuredClone(obj)
来源：http://hz.yuanzhike.top/gtzypgoskq.html

[U93] JS：模板字符串
来源：http://hz.chenlongwang.top/gttgdcqjgr.html

`共 ${n} 条`
来源：http://hz.fengsongda.top/gtxkpkxtpc.html

[U94] JS：箭头函数
来源：http://hz.zhijiandao.cn/gtmzwihmud.html

const double = x => x * 2;
来源：http://hz.svipenyu.cn/gtbsugezpv.html

[U95] JS：Promise 包装
来源：http://hz.xuanzx.com/gtqxzsxyhg.html

new Promise((resolve, reject) => {})
来源：http://hz.meibo888.top/gtrhtdsnka.html

[U96] JS：async/await 与异常
来源：http://hz.cqqwz.cn/gtluuizysq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtevxtbcpv.html

[U97] JS：并发请求
来源：http://hz.tianlin.xyz/gtyovbvzsg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtvwwgnmkw.html

[U98] JS：fetch 带 JSON
来源：http://hz.yonumen.top/gtmdnzyjtg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jlsjyb.cn/gthhtjurqw.html

[U99] JS：事件监听
来源：http://hz.yj20258.top/gtjvkhwkgm.html

el.addEventListener("click", e => {})
来源：http://hz.havefunace.top/gttazfxffi.html

[U100] JS：DOM 查询
来源：http://hz.feifeiyinyue.top/gtndzpjosc.html

document.querySelector(".item")
来源：http://hz.ehwqpu.com/gthvnlitgb.html

[U101] JS：classList 操作
来源：http://hz.zdqjudy.top/gttqdtapkg.html

el.classList.toggle("active")
来源：http://hz.ybcxt.top/gtdpqgasgs.html

[U102] JS：本地存储
来源：http://hz.shanyushiyangkeji.top/gtqdxuikqz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhongyouzk.top/gtpgcrwbwd.html

[U103] JS：定时器
来源：http://hz.yueranfly.top/gtconkklcm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.c1oappe.top/gtpshbuoct.html

[U104] JS：防抖
来源：http://hz.tian-w.cn/gtbmdsskaz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtxddabqco.html

[U105] JS：节流
来源：http://hz.fzhhl.top/gtaebfwhod.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hysaishi.cn/gtynsmxgyi.html

[U106] JS：日期格式化
来源：http://hz.chenjidiqi.icu/gtmlfrhgtb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ivvv.top/gtemopwmmu.html

[U107] JS：数字千分位
来源：http://hz.yj202588.top/gtvhvgmgqf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.feifeiyinyue.top/gteqktixwo.html

[U108] JS：随机整数
来源：http://hz.quarkkingdee.top/gtpudjcpor.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.nwbrower.top/gtkkkqnibf.html

[U109] JS：数组分组
来源：http://hz.yj20258.top/gtdthwjycy.html

Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gtonxyvsoz.html

[U110] JS：数组分块
来源：http://hz.nanxuanxn.top/gtjwphlfdj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yonumen.top/gtdmffigft.html

[U111] JS：对象转 Map
来源：http://hz.aizwys.cn/gtakgztrqc.html

new Map(Object.entries(obj))
来源：http://hz.sysykeji.top/gtrezxdixq.html

[U112] JS：字符串补位
来源：http://hz.birdmap.top/gtywnzpjor.html

"7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtkaimgqpj.html

[U113] JS：正则替换全部
来源：http://hz.zhoulong.xyz/gtqaozooak.html

s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtamzlxjbd.html

[U114] JS：JSON 深比较
来源：http://hz.aizwys.cn/gtcswjwrbl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gtmbenxppo.html

[U115] JS：生成 UUID
来源：http://hz.yj20258.top/gtbjkwmfxw.html

crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtdoigfjek.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.haohaochexian.top/gtxqfgmwqz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zycfv.cn/gtralfajmh.html

[U117] JS：单元测试
来源：http://hz.ydzc1.top/gtyyvdkhjr.html

npm i -D vitest;  npx vitest
来源：http://hz.shzxlz.cn/gtnvenxunk.html

[U118] JS：开发服务器
来源：http://hz.shanyushiyangtech.top/gtagjugnso.html

npm i -D vite;  npx vite
来源：http://hz.pengpengdd.cyou/gtqkxkpwbc.html

[U119] JS：生产构建
来源：http://hz.xylfe.cn/gtbfrqiutz.html

npx vite build
来源：http://hz.9152youxi.cn/gtbtskijtq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sxryk.cn/gtevwctpbk.html

import.meta.env.VITE_API_URL
来源：http://hz.hnxiangtu.top/gtshqiuude.html

================================================================================
来源：http://hz.cucudq.cn/gtdqiwoxiq.html

统计汇总
来源：http://hz.jyoumei.cn/gthhsdqslt.html

================================================================================
来源：http://hz.hywenlv.cn/gtzvvdobak.html

按语言统计（条）：
来源：http://hz.jiagoushi.top/gttaubvuwi.html

Python ......... 252
来源：http://hz.yueranfly.top/gtycfhobhw.html

PHP ............ 252
来源：http://hz.ydzc1.top/gtxvqtgnhj.html

JavaScript ..... 252
来源：http://hz.snrcjt.cn/gtypdzkmel.html

TypeScript ..... 212
来源：http://hz.tian-w.cn/gtwwmdhefp.html

Java ........... 212
来源：http://hz.tian-w.cn/gtkaqbfbmh.html

Go ............. 212
来源：http://hz.dianchejie.cn/gtbciiaooh.html

Ruby ........... 212
来源：http://hz.yuxming.cn/gtpjlriuqz.html

C# ............. 212
来源：http://hz.yueranfly.top/gtstctovke.html

C .............. 30
来源：http://hz.hnxiangtu.top/gtgokvbvyr.html

C++ ............ 30
来源：http://hz.ydzc1.top/gtenxztnjd.html

SQL ............ 90
来源：http://hz.jlsjyb.cn/gtezvoyllq.html

Bash ........... 80
来源：http://hz.hywenlv.cn/gtnafxmbvp.html

Kotlin ......... 15
来源：http://hz.c1oappe.top/gtqbbsqzdw.html

Swift .......... 15
来源：http://hz.andypj.xyz/gtufprprua.html

Lua ............ 10
来源：http://hz.tian-w.cn/gtysxldabr.html

Perl ........... 10
来源：http://hz.yj20258888.top/gtzlzvthzv.html

Scala .......... 10
来源：http://hz.birdmap.top/gtpjarszbf.html

------------------------------------
来源：http://hz.ydzc1.top/gteuebozro.html

合计 ........... 2106 条
来源：http://hz.ybcxt.top/gtqtwhytth.html

按章节统计：
来源：http://hz.redwolf501.top/gtrnojxayd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.dianchejie.cn/gtbfnfhlbs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtzctobrif.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yj20258.top/gtuedbufop.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xingfuxueyuan.xyz/gtmmevbyvc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nanxinkj.top/gtgfqejzrk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ivvv.top/gtlqecpnuk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhiwuduotai.top/gtsnhaxwnw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hnqzz.top/gttmnjcdab.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtlpakchlk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ywan-chungtsiang.top/gtikydrvmm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtdxonrqwa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtjkvqixsf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtsegmfnqv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtbljfxxja.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tianlin.xyz/gtzgxusxhh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtpinlwljm.html

Q SQL 专题                              90
来源：http://hz.haohaochexian.top/gtotowvoel.html

R Bash 专题                             80
来源：http://hz.xinyue.icu/gtrfvehiwk.html

S C / C++ 专题                          60
来源：http://hz.xylfe.cn/gtsgtmwket.html

T 其他语言补充                          60
来源：http://hz.zhongyouzk.top/gtvqvsjcvc.html

U 高频实用片段                         120
来源：http://hz.yuxming.cn/gthvzmxeqe.html

------------------------------------
来源：http://hz.yuxming.cn/gtatiensym.html

合计                                  2106 条
来源：http://hz.jlsjyb.cn/gtmofnriul.html

--------------------------------------------------------------------------------
来源：http://hz.ivvv.top/gtrpbezzdo.html


<!-- 参考信息 -->