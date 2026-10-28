代发 wailian999

case class User(name: String, age: Int)
来源：http://hz.kuanghao11.cn/gtcwfnxuxv.html

[T57] Scala：模式匹配
来源：http://hz.sysykeji.top/gtefmfnqsp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jianghu66.top/gtrlhmmctc.html

[T58] Scala：函数定义
来源：http://hz.yongpay.top/gtohhbpnjm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.meibo888.top/gtmbkihedp.html

[T59] Scala：循环
来源：http://hz.zhoulong.xyz/gtddfgxhpq.html

for (i <- 1 to 10) println(i)
来源：http://hz.guannengcc.top/gtuuzcvytw.html

[T60] Scala：折叠
来源：http://hz.sysykeji.top/gtuqeffebx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ivvv.top/gtmwdwhuce.html

================================================================================
来源：http://hz.dashuyun.cn/gtusrpayzh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yonumen.top/gtnhxmlvfv.html

================================================================================
来源：http://hz.gzhubu.top/gtmwnnigpe.html

[U01] Py：创建虚拟环境
来源：http://hz.yvedp.cn/gtnrogbppk.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zdqjudy.top/gtubbamfqd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yuanzhike.top/gtsbiafjjl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jqgfzy.top/gtqdaozlhr.html

[U03] Py：加载 .env 配置
来源：http://hz.jinghuilouyu.cn/gtrceepenl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj20258888.top/gttvcadbyv.html

[U04] Py：变量调试打印
来源：http://hz.chenjidiqi.icu/gtthqaizyn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dashuyun.cn/gtfcvqhsgu.html

[U05] Py：列表去重且保序
来源：http://hz.cqqwz.cn/gtwsrugtnl.html

list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gttszprred.html

[U06] Py：合并两个字典
来源：http://hz.jqgfzy.top/gtevuvvncz.html

{**a, **b}
来源：http://hz.jyoumei.cn/gtosvpushk.html

[U07] Py：反转字典键值
来源：http://hz.tianlin.xyz/gthhxvvrbx.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gtrsyatiec.html

[U08] Py：展平二维列表
来源：http://hz.fengsongda.top/gtrabijjyy.html

[y for x in nested for y in x]
来源：http://hz.guowangkeji.top/gtkuaqxhoa.html

[U09] Py：字典取最大值的键
来源：http://hz.yuanzhike.top/gtstivxags.html

max(d, key=d.get)
来源：http://hz.xziqi.cn/gtnosfaauf.html

[U10] Py：按值排序字典
来源：http://hz.feifeiyinyue.top/gtmzvkjwqz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hongshengwenyu.top/gtgcfurahb.html

[U11] Py：生成器表达式
来源：http://hz.dianchejie.cn/gtgmazrjux.html

(x * 2 for x in arr)
来源：http://hz.xingfuxueyuan.xyz/gtbvmljieo.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xinyue.icu/gtrvwdjduz.html

Counter(arr).most_common(3)
来源：http://hz.iojbl.cn/gtflanhmjb.html

[U13] Py：固定长度队列
来源：http://hz.haohaochexian.top/gthfvekfah.html

deque(maxlen=10)
来源：http://hz.ppjwa.cn/gtiykdysfp.html

[U14] Py：分组收集到列表
来源：http://hz.zhixingplan.top/gtefmxwdkt.html

defaultdict(list)
来源：http://hz.cashguo.top/gtvqvfwuia.html

[U15] Py：高精度计时
来源：http://hz.52xcode.cn/gtqmlljbec.html

t = time.perf_counter()
来源：http://hz.cashguo.top/gthhcnytet.html

[U16] Py：命令行参数解析
来源：http://hz.daria6918.cn/gtacjwxcfz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ybcxt.top/gtyuiieitw.html

[U17] Py：初始化日志
来源：http://hz.xinyue.icu/gtgatjgcyq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fengsongda.top/gtdwwttzib.html

[U18] Py：预编译正则
来源：http://hz.tian-w.cn/gtatsdrggc.html

pat = re.compile(r"\d+")
来源：http://hz.xingfuxueyuan.xyz/gtoagbvuit.html

[U19] Py：正则替换带回调
来源：http://hz.smart0.xyz/gtwqianafm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.dianchejie.cn/gtygmvxzhv.html

[U20] Py：缓存函数结果
来源：http://hz.chenzaomai.com/gtarmgzrrf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.fzhhl.top/gtwjhgkskw.html

[U21] Py：自定义上下文管理器
来源：http://hz.kuanghao11.cn/gthvxntvot.html

@contextlib.contextmanager
来源：http://hz.jinghuilouyu.cn/gtfdokfpvm.html

[U22] Py：矩阵转置
来源：http://hz.ehwqpu.com/gtmuwbolpt.html

list(zip(*m))
来源：http://hz.yongpay.top/gtzpmvwhwo.html

[U23] Py：分块读取大文件
来源：http://hz.xingfuxueyuan.xyz/gtjfgexmqp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yj20258.top/gttnzkiiqc.html

[U24] Py：路径操作
来源：http://hz.jinqigfzy.top/gtievcbtmu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.andypj.xyz/gtrljftqde.html

[U25] Py：CSV 按字典读
来源：http://hz.yj202588.top/gtiexutyby.html

csv.DictReader(f)
来源：http://hz.jinyuanbaomall.cn/gtcclksqsz.html

[U26] Py：并发下载
来源：http://hz.gaohongyu789.top/gtibqxietc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.svipenyu.cn/gtjlnxiltr.html

[U27] Py：异步 HTTP
来源：http://hz.zhengqikj.top/gteejlqwbo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yuxming.cn/gtdprkrwhg.html

[U28] Py：类型别名
来源：http://hz.mhx1999.top/gtslhnhudz.html

UserId = int
来源：http://hz.xuanzx.com/gtakhfupsr.html

[U29] Py：属性校验
来源：http://hz.jqgfzy.top/gtaatlqhma.html

@property 与 @x.setter 配合
来源：http://hz.hfpthk.cn/gtsfubefcx.html

[U30] Py：数据类
来源：http://hz.chenzaomai.com/gtgsggvzww.html

@dataclass(slots=True)
来源：http://hz.redwolf501.top/gtatmxsbns.html

[U31] Py：单测
来源：http://hz.jqgfzy.top/gtyvpbeizj.html

python -m pytest -q
来源：http://hz.zhengqikj.top/gtfrzlqvfx.html

[U32] Py：代码格式化
来源：http://hz.52xcode.cn/gtavmktqze.html

ruff format . && ruff check --fix .
来源：http://hz.gaohongyu789.top/gtixtheaga.html

[U33] Py：打包发布
来源：http://hz.ybcxt.top/gtblddsgwq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.pengpengdd.cyou/gtazhezdnq.html

[U34] Py：判断编码
来源：http://hz.zdqjudy.top/gtuvbrljqu.html

chardet.detect(raw)
来源：http://hz.c1oappe.top/gteuujdimq.html

[U35] Py：发送邮件
来源：http://hz.pycfn.com/gtfhzuxcxr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zdqjudy.top/gtdzzhrtwo.html

[U36] Py：定时任务
来源：http://hz.cheryme.top/gtezmjfyaa.html

schedule.every(10).minutes.do(job)
来源：http://hz.daxiang520.top/gtbivpqvgk.html

[U37] Py：读写 Excel
来源：http://hz.daxiang520.top/gtzgliyuiq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.haohaochexian.top/gtyimxonkr.html

[U38] Py：获取脚本所在目录
来源：http://hz.hammf.cn/gtbrsikvwj.html

Path(__file__).resolve().parent
来源：http://hz.zhoulong.xyz/gtbuqqlxog.html

[U39] Py：判断是否在交互环境
来源：http://hz.wangdashe.top/gtvavqutjt.html

sys.stdout.isatty()
来源：http://hz.yongpay.top/gtsxiudpxa.html

[U40] Py：打印到标准错误
来源：http://hz.cqqwz.cn/gtvwweyigl.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtevpjmejn.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xziqi.cn/gtqzdrtqpb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.52xcode.cn/gtpbxsxgxb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.birdmap.top/gtgbwuvnlv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pengpengdd.cyou/gtcpdxaufa.html

[U43] PHP：声明命名空间
来源：http://hz.zdqjudy.top/gtojfsmpcv.html

namespace App\Http;
来源：http://hz.ybcxt.top/gtcrfakasv.html

[U44] PHP：开启严格类型
来源：http://hz.tanke756.top/gtryahoiqu.html

declare(strict_types=1);
来源：http://hz.nanxuanxn.top/gtapqzlorr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhengqikj.top/gtkzeqlnwg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtmptlcscp.html

[U46] PHP：可空类型
来源：http://hz.meibo888.top/gtpvaeqqjn.html

?string $name = null
来源：http://hz.redwolf501.top/gtkrldklud.html

[U47] PHP：联合类型
来源：http://hz.wangshuangyany.cn/gtubdgfajb.html

int|string $id
来源：http://hz.jinyuanbaomall.cn/gttogqxhfz.html

[U48] PHP：纯枚举
来源：http://hz.yuxming.cn/gtsnbrbzmb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.c1oappe.top/gtartofgcu.html

[U49] PHP：只读属性
来源：http://hz.wangshuangyany.cn/gtiykgxkgx.html

public readonly string $name
来源：http://hz.jinyuanbaomall.cn/gtgtoahvzr.html

[U50] PHP：构造器属性提升
来源：http://hz.chenzaomai.com/gtapwmvuut.html

public function __construct(private int $id) {}
来源：http://hz.hnxiangtu.top/gtlyftison.html

[U51] PHP：数组解构
来源：http://hz.zhoulong.xyz/gtvdzfdvcy.html

[$a, $b] = $arr;
来源：http://hz.52xcode.cn/gtgejngycm.html

[U52] PHP：箭头函数
来源：http://hz.jinghuilouyu.cn/gtmgrhhjnk.html

$double = fn($x) => $x * 2;
来源：http://hz.dashuyun.cn/gtxvhzgizs.html

[U53] PHP：空合并运算符
来源：http://hz.birdmap.top/gtuxvojubb.html

$v = $a ?? $b ?? "default";
来源：http://hz.cheryme.top/gtfheshnqm.html

[U54] PHP：空安全调用
来源：http://hz.pengpengdd.cyou/gtoxhubgbm.html

$obj?->method()
来源：http://hz.daxiang520.top/gtigiaikdj.html

[U55] PHP：match 表达式
来源：http://hz.cqqwz.cn/gtjgyuagvk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.wangshuangyany.cn/gtirfgwltl.html

[U56] PHP：命名参数
来源：http://hz.ydzc1.top/gtiwqsffuz.html

f(a: 1, b: 2)
来源：http://hz.yongpay.top/gttmbvwzgu.html

[U57] PHP：字符串插值
来源：http://hz.bjfxy.top/gtkisinmck.html

"值: {$a}"
来源：http://hz.redwolf501.top/gttpcnvlhs.html

[U58] PHP：数组三件套
来源：http://hz.shuidangran.top/gtfmsythxq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.havefunace.top/gtycutabrx.html

[U59] PHP：自定义排序
来源：http://hz.yonumen.top/gtmbhcajcb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xingfuxueyuan.xyz/gthfhnnpfs.html

[U60] PHP：JSON 编解码
来源：http://hz.316326.xyz/gtrnaenqkv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hfpthk.cn/gtqkqqvfmx.html

[U61] PHP：正则
来源：http://hz.hammf.cn/gtjxenzpsb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gtwrlsdicn.html

[U62] PHP：日期对象
来源：http://hz.chenzaomai.com/gtfhwszvhh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.9152youxi.cn/gtmutvwpzt.html

[U63] PHP：文件读写
来源：http://hz.aibaodan.cn/gthojesiqp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cdnleiting.top/gtfpoexmin.html

[U64] PHP：目录遍历
来源：http://hz.shanyushiyangkeji.top/gtevedrirk.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnxiangtu.top/gtlahvbckb.html

[U65] PHP：会话
来源：http://hz.xuetiantiany.cn/gtooivylhu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shzxlz.cn/gtzebyasgj.html

[U66] PHP：设置 Cookie
来源：http://hz.pengpengdd.cyou/gtdspvzehv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuxming.cn/gtxwuhdxsg.html

[U67] PHP：处理文件上传
来源：http://hz.quarkkingdee.top/gtjygvfxiq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ivvv.top/gtpfstrvta.html

[U68] PHP：PDO 连接
来源：http://hz.zhoulong.xyz/gtdoioslws.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.daxiang520.top/gtbdmpvknb.html

[U69] PHP：PDO 预处理
来源：http://hz.chenlongwang.top/gtzgktynuq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cashguo.top/gteivxtmrj.html

[U70] PHP：PDO 事务
来源：http://hz.shanyushiyangkeji.top/gtomketiwa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.aibaodan.cn/gtxpmkahxk.html

[U71] PHP：抛出异常
来源：http://hz.gotoacloud.top/gtuecyabyx.html

throw new RuntimeException("失败", 500);
来源：http://hz.zycfv.cn/gttvuabjqy.html

[U72] PHP：写错误日志
来源：http://hz.jinqigufen.top/gtklkgtmip.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yj20258.top/gtmbhmbmsi.html

[U73] PHP：读取 ini 配置
来源：http://hz.vqdsnc.cn/gtdgdceccy.html

parse_ini_file("config.ini", true)
来源：http://hz.guannengcc.top/gtxfyclpja.html

[U74] PHP：读取环境变量
来源：http://hz.yonumen.top/gtomauabfo.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gogol.net.cn/gtxuiqbvsv.html

[U75] PHP：依赖注入
来源：http://hz.cashguo.top/gtyhiamqow.html

composer require psr/container
来源：http://hz.jinqigufen.top/gtdfllcsru.html

[U76] PHP：简单路由
来源：http://hz.redwolf501.top/gtflcmaxeo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.dianchejie.cn/gtzonohzfu.html

[U77] PHP：模板渲染
来源：http://hz.sysykeji.top/gtdxnbmkdp.html

composer require twig/twig
来源：http://hz.wangdashe.top/gtfcdyjcuo.html

[U78] PHP：单元测试
来源：http://hz.jlsjyb.cn/gtlmhabknd.html

composer require --dev phpunit/phpunit
来源：http://hz.zhiwuduotai.top/gtbhneuyul.html

[U79] PHP：静态分析
来源：http://hz.ydjk.org.cn/gtvtyibqzv.html

composer require --dev phpstan/phpstan
来源：http://hz.ydzc1.top/gtavrpvuid.html

[U80] PHP：代码规范修复
来源：http://hz.jinghuilouyu.cn/gtjstewlga.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhijiandao.cn/gtlyjhoxdx.html

[U81] JS：初始化项目
来源：http://hz.jqgufenzy.top/gtexexdeqd.html

npm init -y;  npm i express
来源：http://hz.andypj.xyz/gtvxdpskqm.html

[U82] JS：package.json 脚本
来源：http://hz.feifeiyinyue.top/gtdcsbehlf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.guowangkeji.top/gtylbdtxoh.html

[U83] JS：ES Module 导入导出
来源：http://hz.chenjidiqi.icu/gtkcztcivg.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj20258888.top/gtndrfaplk.html

[U84] JS：CommonJS 写法
来源：http://hz.yuxming.cn/gtxwbzcyyk.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cheryme.top/gtjisafigm.html

[U85] JS：可选链
来源：http://hz.gzhubu.top/gthasfhirq.html

a?.b?.c
来源：http://hz.quarkkingdee.top/gtuffiqmij.html

[U86] JS：空值合并
来源：http://hz.gzhubu.top/gttmntobkq.html

a ?? b
来源：http://hz.pengpengdd.cyou/gtdlpgzqfu.html

[U87] JS：解构默认值
来源：http://hz.ywan-chungtsiang.top/gtfgldtmap.html

const { a = 1, b = 2 } = obj;
来源：http://hz.haohaochexian.top/gttyoeydaw.html

[U88] JS：对象展开合并
来源：http://hz.jianghu66.top/gtrxnoaywj.html

{ ...a, ...b }
来源：http://hz.ydzc1.top/gtqrntkyjy.html

[U89] JS：数组去重
来源：http://hz.yj20258.top/gtrsftxaum.html

[...new Set(arr)]
来源：http://hz.svipenyu.cn/gtergyyuys.html

[U90] JS：数字数组排序
来源：http://hz.vqdsnc.cn/gtljwwfmyz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtzpbriays.html

[U91] JS：对象键值遍历
来源：http://hz.daxiang520.top/gtcyiavanw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shangyingyoupin.top/gtxlsadvdu.html

[U92] JS：深拷贝
来源：http://hz.316326.xyz/gtuqnjlulw.html

structuredClone(obj)
来源：http://hz.hysaishi.cn/gtyfyjrgap.html

[U93] JS：模板字符串
来源：http://hz.yj20258888.top/gtjhkjrlcm.html

`共 ${n} 条`
来源：http://hz.ppjwa.cn/gtevlamxcq.html

[U94] JS：箭头函数
来源：http://hz.hongshengwenyu.top/gtfuqrocrp.html

const double = x => x * 2;
来源：http://hz.sufxvd.cn/gtqmbaxahl.html

[U95] JS：Promise 包装
来源：http://hz.ivvv.top/gtetwbwtlg.html

new Promise((resolve, reject) => {})
来源：http://hz.haohaochexian.top/gtjqqyqfal.html

[U96] JS：async/await 与异常
来源：http://hz.jqgufenzy.top/gtyzuumcod.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hammf.cn/gthgvcopkm.html

[U97] JS：并发请求
来源：http://hz.gogol.net.cn/gtipupqcwg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtwexojblu.html

[U98] JS：fetch 带 JSON
来源：http://hz.sufxvd.cn/gtpijffvjp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.sxryk.cn/gtxvexynbo.html

[U99] JS：事件监听
来源：http://hz.hnqzz.top/gtgydgzsmw.html

el.addEventListener("click", e => {})
来源：http://hz.hysaishi.cn/gttwnuwpgk.html

[U100] JS：DOM 查询
来源：http://hz.shzxlz.cn/gtkcswmwqp.html

document.querySelector(".item")
来源：http://hz.zhengqikj.top/gtnfpszdiq.html

[U101] JS：classList 操作
来源：http://hz.zhijiandao.cn/gtudrxotbm.html

el.classList.toggle("active")
来源：http://hz.yueranfly.top/gtpjmksebt.html

[U102] JS：本地存储
来源：http://hz.zhoulong.xyz/gtxplefqyq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.c1oappe.top/gtnowbdkut.html

[U103] JS：定时器
来源：http://hz.yj202588.top/gtnzuhoalr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jiagoushi.top/gtrjgzvehz.html

[U104] JS：防抖
来源：http://hz.fzhhl.top/gtjwndrjou.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtblgvwbuf.html

[U105] JS：节流
来源：http://hz.yuxming.cn/gtpkmsdalm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xylfe.cn/gtpbibrwlw.html

[U106] JS：日期格式化
来源：http://hz.xuanzx.com/gtfiuucjnz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yongpay.top/gtfdsulsnt.html

[U107] JS：数字千分位
来源：http://hz.c1oappe.top/gtlfguhgmx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gogol.net.cn/gtsovpbqoz.html

[U108] JS：随机整数
来源：http://hz.chenlongwang.top/gtgagfdlaf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhiwuduotai.top/gtebfykblk.html

[U109] JS：数组分组
来源：http://hz.gaohongyu789.top/gtysidqjqn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtzwafsuml.html

[U110] JS：数组分块
来源：http://hz.0kj1m.cn/gtfxiasiym.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gaohongyu789.top/gtynsivdtp.html

[U111] JS：对象转 Map
来源：http://hz.birdmap.top/gtvradzbdy.html

new Map(Object.entries(obj))
来源：http://hz.zdqjudy.top/gturrhtuqx.html

[U112] JS：字符串补位
来源：http://hz.jqgufenzy.top/gtauvjszby.html

"7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtyeuhlsrb.html

[U113] JS：正则替换全部
来源：http://hz.yuanzhike.top/gtfoiizyfg.html

s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtahdtubyu.html

[U114] JS：JSON 深比较
来源：http://hz.shangyingyoupin.top/gtfwqkiulf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtjedkwpzp.html

[U115] JS：生成 UUID
来源：http://hz.jinghuilouyu.cn/gttpfdjhum.html

crypto.randomUUID()
来源：http://hz.cashguo.top/gtwtdvgcxq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cucudq.cn/gtdtpmkojf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hnqzz.top/gtesrighdm.html

[U117] JS：单元测试
来源：http://hz.fengsongda.top/gthzsvomzx.html

npm i -D vitest;  npx vitest
来源：http://hz.zhoulong.xyz/gtaiuiyiwh.html

[U118] JS：开发服务器
来源：http://hz.shanyushiyangkeji.top/gtmkicxsza.html

npm i -D vite;  npx vite
来源：http://hz.ywan-chungtsiang.top/gtjfljjrqj.html

[U119] JS：生产构建
来源：http://hz.pengpengdd.cyou/gtunyidtzq.html

npx vite build
来源：http://hz.fzhhl.top/gtdoyyiemj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yangfankeji.com/gtwofrzxil.html

import.meta.env.VITE_API_URL
来源：http://hz.9152youxi.cn/gtenhjwctg.html

================================================================================
来源：http://hz.cheryme.top/gtsdihoxgh.html

统计汇总
来源：http://hz.jqgfzy.top/gtsezasuzv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgepbrhqk.html

按语言统计（条）：
来源：http://hz.redwolf501.top/gttkmswxca.html

Python ......... 252
来源：http://hz.cqqwz.cn/gtakogocdk.html

PHP ............ 252
来源：http://hz.ydzc1.top/gtlbxqdujv.html

JavaScript ..... 252
来源：http://hz.hnqzz.top/gtvfisovxf.html

TypeScript ..... 212
来源：http://hz.mhx1999.top/gtwttwvmra.html

Java ........... 212
来源：http://hz.hnqzz.top/gtzidkypku.html

Go ............. 212
来源：http://hz.andypj.xyz/gtsngggtgq.html

Ruby ........... 212
来源：http://hz.snrcjt.cn/gtduqkeyem.html

C# ............. 212
来源：http://hz.yanxiufei.cn/gtmpyflkqu.html

C .............. 30
来源：http://hz.jinyuanbaomall.cn/gtvlfzehbu.html

C++ ............ 30
来源：http://hz.cdnleiting.top/gtrxxutcin.html

SQL ............ 90
来源：http://hz.yangfankeji.com/gtqsrmegal.html

Bash ........... 80
来源：http://hz.tanke756.top/gtkfzkkmgp.html

Kotlin ......... 15
来源：http://hz.ywan-chungtsiang.top/gtnrttxrqi.html

Swift .......... 15
来源：http://hz.sxryk.cn/gtdrynouyu.html

Lua ............ 10
来源：http://hz.gogol.net.cn/gtsvnxnpkj.html

Perl ........... 10
来源：http://hz.bjfxy.top/gtccmoujzn.html

Scala .......... 10
来源：http://hz.redwolf501.top/gtaczvukpd.html

------------------------------------
来源：http://hz.yvedp.cn/gtqmfcghbr.html

合计 ........... 2106 条
来源：http://hz.tian-w.cn/gtoycsehev.html

按章节统计：
来源：http://hz.sxryk.cn/gtrlrwrouz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.mhx1999.top/gtlelpelpx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.quarkkingdee.top/gtftaxzlze.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sufxvd.cn/gtgpgauzcf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zdqjudy.top/gtbvrygekm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.0kj1m.cn/gtymvtetkr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yueranfly.top/gtqgpofwht.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sxryk.cn/gtxpxhfpxt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtvjnfrzpi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtzcyskaih.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinghuilouyu.cn/gtuyojzthv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtjuglkyzb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtfbagzqjf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtxsnnzcis.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.fzhhl.top/gtgaicmuom.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhengqikj.top/gthtnqlaiz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtuogyxhem.html

Q SQL 专题                              90
来源：http://hz.yuanzhike.top/gtvtkgmqol.html

R Bash 专题                             80
来源：http://hz.52xcode.cn/gtteppsfpy.html

S C / C++ 专题                          60
来源：http://hz.shangyingyoupin.top/gtrnkyucnk.html

T 其他语言补充                          60
来源：http://hz.cheryme.top/gtcsocuwdk.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangkeji.top/gtxrtllhke.html

------------------------------------
来源：http://hz.vqdsnc.cn/gtenprnasi.html

合计                                  2106 条
来源：http://hz.jiagoushi.top/gtcivpniti.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtemletnui.html


<!-- 参考信息 -->