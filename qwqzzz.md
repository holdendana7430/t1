代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sxryk.cn/gtadscbwgi.html

[T59] Scala：循环
来源：http://hz.shuidangran.top/gtauovslrw.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhoulong.xyz/gtzgyowlpc.html

[T60] Scala：折叠
来源：http://hz.zhongyouzk.top/gtsznckrbw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.dianchejie.cn/gtawrcpjip.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtoudyiltu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.dashuyun.cn/gtygufsxxo.html

================================================================================
来源：http://hz.yonumen.top/gtxfvqrubv.html

[U01] Py：创建虚拟环境
来源：http://hz.hongshengwenyu.top/gtkqwskdtl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yanxiufei.cn/gtmsvrhalh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hywenlv.cn/gtoaplmmxu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xylfe.cn/gteurgufnb.html

[U03] Py：加载 .env 配置
来源：http://hz.kuanghao11.cn/gtutjkbxip.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.havefunace.top/gtbuyjorpk.html

[U04] Py：变量调试打印
来源：http://hz.shzxlz.cn/gthmjesbfy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yangfankeji.com/gtanciyhoe.html

[U05] Py：列表去重且保序
来源：http://hz.hfpthk.cn/gtucxracye.html

list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gthbwlrsct.html

[U06] Py：合并两个字典
来源：http://hz.9152youxi.cn/gtnfbmilky.html

{**a, **b}
来源：http://hz.zhongyouzk.top/gtdbhfkvbu.html

[U07] Py：反转字典键值
来源：http://hz.sufxvd.cn/gtarululnb.html

{v: k for k, v in d.items()}
来源：http://hz.cashguo.top/gtcpkamnft.html

[U08] Py：展平二维列表
来源：http://hz.0kj1m.cn/gtcdadhzfu.html

[y for x in nested for y in x]
来源：http://hz.shangyingyoupin.top/gtgdpoxndi.html

[U09] Py：字典取最大值的键
来源：http://hz.havefunace.top/gtfxowgxvv.html

max(d, key=d.get)
来源：http://hz.andypj.xyz/gtwvuoxldt.html

[U10] Py：按值排序字典
来源：http://hz.yvedp.cn/gteijpinvx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jqgfzy.top/gtnblscndb.html

[U11] Py：生成器表达式
来源：http://hz.cucudq.cn/gtelnpbiax.html

(x * 2 for x in arr)
来源：http://hz.ivvv.top/gtxaveigeu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.guannengcc.top/gtyikopsbv.html

Counter(arr).most_common(3)
来源：http://hz.xingfuxueyuan.xyz/gtbtiourpr.html

[U13] Py：固定长度队列
来源：http://hz.andypj.xyz/gtzznretcp.html

deque(maxlen=10)
来源：http://hz.snrcjt.cn/gtnuupmsqn.html

[U14] Py：分组收集到列表
来源：http://hz.yonumen.top/gtseklafgw.html

defaultdict(list)
来源：http://hz.chenjidiqi.icu/gtrehshzdw.html

[U15] Py：高精度计时
来源：http://hz.zhengqikj.top/gtyftpghev.html

t = time.perf_counter()
来源：http://hz.yj20258.top/gtiaexrsho.html

[U16] Py：命令行参数解析
来源：http://hz.xylfe.cn/gtoyrmvawd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.0kj1m.cn/gtwuphboyh.html

[U17] Py：初始化日志
来源：http://hz.yanxiufei.cn/gtagqxzqjf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fzhhl.top/gtxctkshxr.html

[U18] Py：预编译正则
来源：http://hz.jinyuanbaomall.cn/gtggdzhzar.html

pat = re.compile(r"\d+")
来源：http://hz.jianghu66.top/gtbbpsjeyk.html

[U19] Py：正则替换带回调
来源：http://hz.quarkkingdee.top/gtdfdfepgh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shanyushiyangtech.top/gtitcpzrgz.html

[U20] Py：缓存函数结果
来源：http://hz.zdqjudy.top/gtztbgodxe.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dianchejie.cn/gtgxudshbw.html

[U21] Py：自定义上下文管理器
来源：http://hz.yangfankeji.com/gtqbchakkt.html

@contextlib.contextmanager
来源：http://hz.mhx1999.top/gtgwdvnfrw.html

[U22] Py：矩阵转置
来源：http://hz.zhiwuduotai.top/gtrqkgclvu.html

list(zip(*m))
来源：http://hz.dianchejie.cn/gteucomfoc.html

[U23] Py：分块读取大文件
来源：http://hz.snrcjt.cn/gtpudzlblf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sysykeji.top/gtsckkgqrj.html

[U24] Py：路径操作
来源：http://hz.pengpengdd.cyou/gtpekyeric.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ppjwa.cn/gtuksrhgxm.html

[U25] Py：CSV 按字典读
来源：http://hz.cheryme.top/gtsbujcqaj.html

csv.DictReader(f)
来源：http://hz.hywenlv.cn/gtiohpocna.html

[U26] Py：并发下载
来源：http://hz.yuanzhike.top/gtkzmkuzuj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.havefunace.top/gtwallmovs.html

[U27] Py：异步 HTTP
来源：http://hz.jinyuanbaomall.cn/gtxtzoujpi.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yongpay.top/gtflasaamx.html

[U28] Py：类型别名
来源：http://hz.nanxinkj.top/gtxxnjfijc.html

UserId = int
来源：http://hz.fzhhl.top/gtnrujovdu.html

[U29] Py：属性校验
来源：http://hz.yuanzhike.top/gtotulkgah.html

@property 与 @x.setter 配合
来源：http://hz.smart0.xyz/gtdkrxuxkk.html

[U30] Py：数据类
来源：http://hz.shanyushiyangkeji.top/gtwvpfspnb.html

@dataclass(slots=True)
来源：http://hz.mhx1999.top/gtsbcahhhf.html

[U31] Py：单测
来源：http://hz.gotoacloud.top/gtvazowzrt.html

python -m pytest -q
来源：http://hz.zhongyouzk.top/gttjgtlzdy.html

[U32] Py：代码格式化
来源：http://hz.redwolf501.top/gtsgupinzs.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtlzmcxefp.html

[U33] Py：打包发布
来源：http://hz.quarkkingdee.top/gttocueuve.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258888.top/gtawhanwkn.html

[U34] Py：判断编码
来源：http://hz.cheryme.top/gticeitupo.html

chardet.detect(raw)
来源：http://hz.meibo888.top/gtsdzdvwhy.html

[U35] Py：发送邮件
来源：http://hz.tian-w.cn/gtgmatufik.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuanzx.com/gtnshdpqra.html

[U36] Py：定时任务
来源：http://hz.xuanzx.com/gtejgasfnp.html

schedule.every(10).minutes.do(job)
来源：http://hz.nwbrower.top/gtltwhqpoi.html

[U37] Py：读写 Excel
来源：http://hz.havefunace.top/gtfrbtimwx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhongyouzk.top/gtwgnouhvv.html

[U38] Py：获取脚本所在目录
来源：http://hz.fengsongda.top/gtnaojxrto.html

Path(__file__).resolve().parent
来源：http://hz.aibaodan.cn/gttbpjwpop.html

[U39] Py：判断是否在交互环境
来源：http://hz.ywan-chungtsiang.top/gtdigzbjnw.html

sys.stdout.isatty()
来源：http://hz.nanxuanxn.top/gtbfpaysvh.html

[U40] Py：打印到标准错误
来源：http://hz.cqqwz.cn/gttcmufikx.html

print("err", file=sys.stderr)
来源：http://hz.redwolf501.top/gtepdmzhux.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gotoacloud.top/gtnhiycmxm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hnxiangtu.top/gtxprluhjz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhongyouzk.top/gtsxohebiv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xingfuxueyuan.xyz/gtaderdwqa.html

[U43] PHP：声明命名空间
来源：http://hz.smart0.xyz/gtgdskaghl.html

namespace App\Http;
来源：http://hz.yj20258888.top/gtxyuyhily.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258.top/gtgaeeqpbi.html

declare(strict_types=1);
来源：http://hz.c1oappe.top/gthkoxvsnl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sufxvd.cn/gtdspmohgy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtdneytmdc.html

[U46] PHP：可空类型
来源：http://hz.xingfuxueyuan.xyz/gtfofysddv.html

?string $name = null
来源：http://hz.tianlin.xyz/gthkwppgxo.html

[U47] PHP：联合类型
来源：http://hz.sxryk.cn/gtrqhucgqj.html

int|string $id
来源：http://hz.zhijiandao.cn/gtgfelmwdt.html

[U48] PHP：纯枚举
来源：http://hz.316326.xyz/gtfktvhhks.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.kuanghao11.cn/gtfxtcbbib.html

[U49] PHP：只读属性
来源：http://hz.vqdsnc.cn/gtvfwdfhva.html

public readonly string $name
来源：http://hz.zhiwuduotai.top/gtphxdruvy.html

[U50] PHP：构造器属性提升
来源：http://hz.guowangkeji.top/gtpiptyxvn.html

public function __construct(private int $id) {}
来源：http://hz.cdnleiting.top/gtlhofoort.html

[U51] PHP：数组解构
来源：http://hz.gzhubu.top/gtocbxivze.html

[$a, $b] = $arr;
来源：http://hz.yvedp.cn/gtwurutecr.html

[U52] PHP：箭头函数
来源：http://hz.zhoulong.xyz/gtsfeldjfz.html

$double = fn($x) => $x * 2;
来源：http://hz.guowangkeji.top/gthvwhvvvd.html

[U53] PHP：空合并运算符
来源：http://hz.birdmap.top/gtpjxzqmsb.html

$v = $a ?? $b ?? "default";
来源：http://hz.yuanzhike.top/gtzdnocmwt.html

[U54] PHP：空安全调用
来源：http://hz.jianghu66.top/gthkgzvfxy.html

$obj?->method()
来源：http://hz.zhaomingkeji.xyz/gtszlepuxr.html

[U55] PHP：match 表达式
来源：http://hz.yuxming.cn/gtoafcnira.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.0kj1m.cn/gtfywebdwz.html

[U56] PHP：命名参数
来源：http://hz.vqdsnc.cn/gtevrjnnpg.html

f(a: 1, b: 2)
来源：http://hz.zhijiandao.cn/gtatziaegv.html

[U57] PHP：字符串插值
来源：http://hz.shuidangran.top/gtimrmdqvk.html

"值: {$a}"
来源：http://hz.tian-w.cn/gtwzfodbyc.html

[U58] PHP：数组三件套
来源：http://hz.ydjk.org.cn/gtkqcmsziw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.quarkkingdee.top/gtumfeqraq.html

[U59] PHP：自定义排序
来源：http://hz.gzhubu.top/gtlhuevmfm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.mhx1999.top/gtqikhzufv.html

[U60] PHP：JSON 编解码
来源：http://hz.chenzaomai.com/gtyefhjqbb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenjidiqi.icu/gtyibacifs.html

[U61] PHP：正则
来源：http://hz.yj20258.top/gtvrzzxdcm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtpaulrsom.html

[U62] PHP：日期对象
来源：http://hz.yj202588.top/gtzabytfgj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aizwys.cn/gtczibibnk.html

[U63] PHP：文件读写
来源：http://hz.mhx1999.top/gtxzvyqlau.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.svipenyu.cn/gteqibivib.html

[U64] PHP：目录遍历
来源：http://hz.jinqigfzy.top/gtskzwtkng.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yangfankeji.com/gtypitauxf.html

[U65] PHP：会话
来源：http://hz.hywenlv.cn/gtuayktvfz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yuanzhike.top/gtwfhuwnjg.html

[U66] PHP：设置 Cookie
来源：http://hz.tian-w.cn/gtsswneqdz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.shanyushiyangtech.top/gtxkwxfahe.html

[U67] PHP：处理文件上传
来源：http://hz.jqgufenzy.top/gtybvywoaa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenlongwang.top/gtddukoyjx.html

[U68] PHP：PDO 连接
来源：http://hz.zhoulong.xyz/gtpuvhlyyr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yangfankeji.com/gtzhyplgxj.html

[U69] PHP：PDO 预处理
来源：http://hz.chenjidiqi.icu/gtruektukt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yanxiufei.cn/gtyhiblgme.html

[U70] PHP：PDO 事务
来源：http://hz.sufxvd.cn/gtkrwamgmc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.haohaochexian.top/gtfxrganqo.html

[U71] PHP：抛出异常
来源：http://hz.zhengqikj.top/gtynnvuyzn.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhixingplan.top/gtmetiwyrz.html

[U72] PHP：写错误日志
来源：http://hz.zhixingplan.top/gtwgmrptdt.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhixingplan.top/gtfcukeagl.html

[U73] PHP：读取 ini 配置
来源：http://hz.hnqzz.top/gtpbrbqcgi.html

parse_ini_file("config.ini", true)
来源：http://hz.chenjidiqi.icu/gtqjdsnczl.html

[U74] PHP：读取环境变量
来源：http://hz.chenjidiqi.icu/gtuphcfzfm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenzaomai.com/gtujyulkhv.html

[U75] PHP：依赖注入
来源：http://hz.aibaodan.cn/gtxgoxuivl.html

composer require psr/container
来源：http://hz.mhx1999.top/gtdcokywmv.html

[U76] PHP：简单路由
来源：http://hz.dashuyun.cn/gtqadoznwc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.daria6918.cn/gtjudewryp.html

[U77] PHP：模板渲染
来源：http://hz.bjfxy.top/gtppqxwefa.html

composer require twig/twig
来源：http://hz.shangyingyoupin.top/gtgyqpwvlx.html

[U78] PHP：单元测试
来源：http://hz.jinqigufen.top/gtaicfhyqk.html

composer require --dev phpunit/phpunit
来源：http://hz.shanyushiyangkeji.top/gtkzqdoxpx.html

[U79] PHP：静态分析
来源：http://hz.birdmap.top/gtphapspwm.html

composer require --dev phpstan/phpstan
来源：http://hz.jlsjyb.cn/gtfihgkjln.html

[U80] PHP：代码规范修复
来源：http://hz.dianchejie.cn/gthtbdqwtd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shanyushiyangtech.top/gtduzmvcfp.html

[U81] JS：初始化项目
来源：http://hz.jinghuilouyu.cn/gtezunihzp.html

npm init -y;  npm i express
来源：http://hz.jiagoushi.top/gtpzwjhcoj.html

[U82] JS：package.json 脚本
来源：http://hz.nanxuanxn.top/gtjvwpjdlc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cashguo.top/gtwfdekuum.html

[U83] JS：ES Module 导入导出
来源：http://hz.316326.xyz/gtjfqjzfnk.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenlongwang.top/gttdheqijb.html

[U84] JS：CommonJS 写法
来源：http://hz.hongshengwenyu.top/gtzftzolxa.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.nanxinkj.top/gtyxpnbnlo.html

[U85] JS：可选链
来源：http://hz.aizwys.cn/gtcbnhrfqz.html

a?.b?.c
来源：http://hz.zhoulong.xyz/gtxdzfgfzf.html

[U86] JS：空值合并
来源：http://hz.svipenyu.cn/gtpuktswib.html

a ?? b
来源：http://hz.cheryme.top/gtvpoyfujs.html

[U87] JS：解构默认值
来源：http://hz.cucudq.cn/gtfptwnhxj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zycfv.cn/gtfsgifzpa.html

[U88] JS：对象展开合并
来源：http://hz.zdqjudy.top/gtmbxgwhzf.html

{ ...a, ...b }
来源：http://hz.dianchejie.cn/gtzumoqeyn.html

[U89] JS：数组去重
来源：http://hz.yongpay.top/gtzlksnhem.html

[...new Set(arr)]
来源：http://hz.yj202588.top/gtupdpncuj.html

[U90] JS：数字数组排序
来源：http://hz.aizwys.cn/gtoruxtovg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtjsulbhyr.html

[U91] JS：对象键值遍历
来源：http://hz.aibaodan.cn/gtteijruvf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.snrcjt.cn/gtmmnzodzv.html

[U92] JS：深拷贝
来源：http://hz.cucudq.cn/gtyfgsbshy.html

structuredClone(obj)
来源：http://hz.shuidangran.top/gtltgbyykw.html

[U93] JS：模板字符串
来源：http://hz.shzxlz.cn/gtmoqajlus.html

`共 ${n} 条`
来源：http://hz.zhijiandao.cn/gthonyscxi.html

[U94] JS：箭头函数
来源：http://hz.jlsjyb.cn/gtxtybmpaf.html

const double = x => x * 2;
来源：http://hz.kuanghao11.cn/gtnfnspgpu.html

[U95] JS：Promise 包装
来源：http://hz.zhiwuduotai.top/gtumitmxpv.html

new Promise((resolve, reject) => {})
来源：http://hz.guannengcc.top/gtecyuthjq.html

[U96] JS：async/await 与异常
来源：http://hz.aizwys.cn/gtnaqjayuc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtglibqhah.html

[U97] JS：并发请求
来源：http://hz.birdmap.top/gtmfiadlqi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtkxkwmrbl.html

[U98] JS：fetch 带 JSON
来源：http://hz.shangyingyoupin.top/gttnrrsehs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhengqikj.top/gtuqsnpfla.html

[U99] JS：事件监听
来源：http://hz.sweek.top/gthuvtrsjx.html

el.addEventListener("click", e => {})
来源：http://hz.zhijiandao.cn/gtprtitqlj.html

[U100] JS：DOM 查询
来源：http://hz.jinyuanbaomall.cn/gtciaojapm.html

document.querySelector(".item")
来源：http://hz.xinyue.icu/gtfnrjblye.html

[U101] JS：classList 操作
来源：http://hz.cqqwz.cn/gtvemyyrbu.html

el.classList.toggle("active")
来源：http://hz.jyoumei.cn/gttkstgyvy.html

[U102] JS：本地存储
来源：http://hz.chenlongwang.top/gtodueyaxe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shangyingyoupin.top/gtqtrheroa.html

[U103] JS：定时器
来源：http://hz.quarkkingdee.top/gtvmguibej.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aibaodan.cn/gtcenzfhwr.html

[U104] JS：防抖
来源：http://hz.zhaomingkeji.xyz/gtbyfmadmn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jiagoushi.top/gthbqenoyw.html

[U105] JS：节流
来源：http://hz.hysaishi.cn/gtrskaggpg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shanyushiyangtech.top/gtiiyauawf.html

[U106] JS：日期格式化
来源：http://hz.zhixingplan.top/gtbxeazoqk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cdnleiting.top/gtfwghwdrr.html

[U107] JS：数字千分位
来源：http://hz.shuidangran.top/gttsnmcvyg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yj20258.top/gthhhsyjps.html

[U108] JS：随机整数
来源：http://hz.tanke756.top/gtvdrszpbr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258.top/gtsamrvtrx.html

[U109] JS：数组分组
来源：http://hz.yj20258888.top/gtqnmximxd.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtkhjtjwmh.html

[U110] JS：数组分块
来源：http://hz.jqgfzy.top/gtppvjrdgc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xuetiantiany.cn/gtopiafhgw.html

[U111] JS：对象转 Map
来源：http://hz.hfpthk.cn/gthklczdrd.html

new Map(Object.entries(obj))
来源：http://hz.cheryme.top/gtsuqhzbdk.html

[U112] JS：字符串补位
来源：http://hz.ivvv.top/gtyuglgjis.html

"7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtckqxfwlp.html

[U113] JS：正则替换全部
来源：http://hz.cdnleiting.top/gtqgvynwjx.html

s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtrwbbvyiv.html

[U114] JS：JSON 深比较
来源：http://hz.aizwys.cn/gtuwcfzjsc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ivvv.top/gtjebywuvc.html

[U115] JS：生成 UUID
来源：http://hz.yvedp.cn/gtijasrffj.html

crypto.randomUUID()
来源：http://hz.meibo888.top/gtjaxtrtaq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sxryk.cn/gtnbyjtwrw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cqqwz.cn/gtahtcmacu.html

[U117] JS：单元测试
来源：http://hz.jinyuanbaomall.cn/gtkybfneqq.html

npm i -D vitest;  npx vitest
来源：http://hz.316326.xyz/gttqlbixin.html

[U118] JS：开发服务器
来源：http://hz.haohaochexian.top/gtyahnztrz.html

npm i -D vite;  npx vite
来源：http://hz.xuetiantiany.cn/gtvetclsbg.html

[U119] JS：生产构建
来源：http://hz.hywenlv.cn/gteqqijrsa.html

npx vite build
来源：http://hz.dashuyun.cn/gtwwvigbtz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ydzc1.top/gtyyhkawtz.html

import.meta.env.VITE_API_URL
来源：http://hz.daria6918.cn/gtorvfdhen.html

================================================================================
来源：http://hz.xziqi.cn/gtevoxojzg.html

统计汇总
来源：http://hz.jianghu66.top/gtajxmuhrx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtojrwiujq.html

按语言统计（条）：
来源：http://hz.yvedp.cn/gtcnuffyjf.html

Python ......... 252
来源：http://hz.yj20258.top/gtiyemtfia.html

PHP ............ 252
来源：http://hz.jinghuilouyu.cn/gtzcptouga.html

JavaScript ..... 252
来源：http://hz.zhengqikj.top/gtsuiqgclp.html

TypeScript ..... 212
来源：http://hz.gzhubu.top/gtnoqkaelp.html

Java ........... 212
来源：http://hz.ehwqpu.com/gthlyrllza.html

Go ............. 212
来源：http://hz.daxiang520.top/gterdpttkt.html

Ruby ........... 212
来源：http://hz.jinqigfzy.top/gtfyqdptys.html

C# ............. 212
来源：http://hz.birdmap.top/gtxekjnzml.html

C .............. 30
来源：http://hz.aizwys.cn/gtajbfndcz.html

C++ ............ 30
来源：http://hz.shzxlz.cn/gtifenkybr.html

SQL ............ 90
来源：http://hz.zhongyouzk.top/gtlxmxgcpp.html

Bash ........... 80
来源：http://hz.yj20258888.top/gtfehnqqbk.html

Kotlin ......... 15
来源：http://hz.yonumen.top/gtmmvckjel.html

Swift .......... 15
来源：http://hz.zycfv.cn/gtpvdpgkrm.html

Lua ............ 10
来源：http://hz.nanxuanxn.top/gtnzwhvmml.html

Perl ........... 10
来源：http://hz.shzxlz.cn/gtdfnuvmxn.html

Scala .......... 10
来源：http://hz.zhijiandao.cn/gtcliqvbqq.html

------------------------------------
来源：http://hz.redwolf501.top/gtzhdpjbff.html

合计 ........... 2106 条
来源：http://hz.yongpay.top/gtsmckpuzl.html

按章节统计：
来源：http://hz.ehwqpu.com/gtjapnvrwz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.52xcode.cn/gtimpogtgf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtjpzqzjau.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtmsakrhdv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sufxvd.cn/gtezbecqyx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.dianchejie.cn/gtmemnghll.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.52xcode.cn/gtdofhbzgg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtoybwcfbr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.havefunace.top/gtxfmhnawi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtnajntisd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hysaishi.cn/gtzujhblrz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gtdtycutxr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtiumctlmf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gttlkyrphr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.guannengcc.top/gtuxcmqvvs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sweek.top/gtyjxkbklk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtpincybxj.html

Q SQL 专题                              90
来源：http://hz.hfpthk.cn/gtyxrvjses.html

R Bash 专题                             80
来源：http://hz.yj202588.top/gtrvddrzhj.html

S C / C++ 专题                          60
来源：http://hz.jinqigfzy.top/gtjxfkvccs.html

T 其他语言补充                          60
来源：http://hz.jinghuilouyu.cn/gtztxtzhki.html

U 高频实用片段                         120
来源：http://hz.yuxming.cn/gtpfxrbsur.html

------------------------------------
来源：http://hz.mhx1999.top/gtgyyixcik.html

合计                                  2106 条
来源：http://hz.9152youxi.cn/gtqhsvrgnc.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtbtenxtpa.html

使用提醒
来源：http://hz.tian-w.cn/gtaensqmyl.html

--------------------------------------------------------------------------------
来源：http://hz.gotoacloud.top/gtwcjnhjni.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhaomingkeji.xyz/gtwavnodlq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.guannengcc.top/gtwdgeelnc.html


<!-- 参考信息 -->