代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuetiantiany.cn/gtsqynraxx.html

[T55] Scala：集合过滤
来源：http://hz.jqgufenzy.top/gtzjbabqmr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sxryk.cn/gtjpxuiwhz.html

[T56] Scala：样例类
来源：http://hz.cdnleiting.top/gtkghegpaq.html

case class User(name: String, age: Int)
来源：http://hz.gaohongyu789.top/gtuaurmyzx.html

[T57] Scala：模式匹配
来源：http://hz.ybcxt.top/gtyubmyjmr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zycfv.cn/gtghzzmugo.html

[T58] Scala：函数定义
来源：http://hz.shzxlz.cn/gtwbrrxfrq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sufxvd.cn/gtovkctuuk.html

[T59] Scala：循环
来源：http://hz.hnxiangtu.top/gtwaboyncr.html

for (i <- 1 to 10) println(i)
来源：http://hz.guowangkeji.top/gtbwdnmwuy.html

[T60] Scala：折叠
来源：http://hz.nanxinkj.top/gtrzbzrhss.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnqzz.top/gtgdqwvqee.html

================================================================================
来源：http://hz.hywenlv.cn/gtobnrzgon.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gttomeavtm.html

================================================================================
来源：http://hz.52xcode.cn/gtebcxgtkz.html

[U01] Py：创建虚拟环境
来源：http://hz.mhx1999.top/gtdvypckcm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nwbrower.top/gtkeiphlfu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shzxlz.cn/gtcrvchjai.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aibaodan.cn/gtplbzmmiy.html

[U03] Py：加载 .env 配置
来源：http://hz.xziqi.cn/gtdviqjtff.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cucudq.cn/gtszqbbszw.html

[U04] Py：变量调试打印
来源：http://hz.hysaishi.cn/gtuchszumv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.fzhhl.top/gtpaivrkla.html

[U05] Py：列表去重且保序
来源：http://hz.shanyushiyangtech.top/gtpiuelxsh.html

list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtycipkyum.html

[U06] Py：合并两个字典
来源：http://hz.shangyingyoupin.top/gtfhhywfgh.html

{**a, **b}
来源：http://hz.snrcjt.cn/gtjictrsha.html

[U07] Py：反转字典键值
来源：http://hz.jqgfzy.top/gtmzvgqaue.html

{v: k for k, v in d.items()}
来源：http://hz.daxiang520.top/gtmyhrbaug.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangkeji.top/gtymmcgjvi.html

[y for x in nested for y in x]
来源：http://hz.zdqjudy.top/gtzzrfdiif.html

[U09] Py：字典取最大值的键
来源：http://hz.meibo888.top/gtchnahvvo.html

max(d, key=d.get)
来源：http://hz.sxryk.cn/gtwwvlopyz.html

[U10] Py：按值排序字典
来源：http://hz.jqgfzy.top/gtledulvmf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ppjwa.cn/gtrlodukww.html

[U11] Py：生成器表达式
来源：http://hz.wangshuangyany.cn/gtfzucnjsl.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gtzxwiskfs.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ivvv.top/gtcgxrvqpt.html

Counter(arr).most_common(3)
来源：http://hz.nwbrower.top/gtpltsukez.html

[U13] Py：固定长度队列
来源：http://hz.hongshengwenyu.top/gtdlrceyei.html

deque(maxlen=10)
来源：http://hz.xuetiantiany.cn/gtktnhaooz.html

[U14] Py：分组收集到列表
来源：http://hz.shzxlz.cn/gtmadrqgbf.html

defaultdict(list)
来源：http://hz.kuanghao11.cn/gtzvvghjjz.html

[U15] Py：高精度计时
来源：http://hz.jianghu66.top/gtfolsomcj.html

t = time.perf_counter()
来源：http://hz.wangshuangyany.cn/gtjhfkbcqd.html

[U16] Py：命令行参数解析
来源：http://hz.jqgufenzy.top/gtfaydsfso.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hysaishi.cn/gtuonvbkhl.html

[U17] Py：初始化日志
来源：http://hz.gotoacloud.top/gtypbqhggn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.dashuyun.cn/gtxudsjwyj.html

[U18] Py：预编译正则
来源：http://hz.yongpay.top/gtbjmgapmm.html

pat = re.compile(r"\d+")
来源：http://hz.iojbl.cn/gteaekenad.html

[U19] Py：正则替换带回调
来源：http://hz.zhijiandao.cn/gtajjkfclp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.guowangkeji.top/gtjcgfyxxv.html

[U20] Py：缓存函数结果
来源：http://hz.iojbl.cn/gtwebhqcit.html

@functools.lru_cache(maxsize=None)
来源：http://hz.pengpengdd.cyou/gtjhgowoht.html

[U21] Py：自定义上下文管理器
来源：http://hz.gogol.net.cn/gtghpclkip.html

@contextlib.contextmanager
来源：http://hz.jyoumei.cn/gtkldfoxsb.html

[U22] Py：矩阵转置
来源：http://hz.snrcjt.cn/gtyxrbuwtq.html

list(zip(*m))
来源：http://hz.zdqjudy.top/gtrskukjsa.html

[U23] Py：分块读取大文件
来源：http://hz.tianlin.xyz/gtgjtvfjix.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sysykeji.top/gtqjeltgyy.html

[U24] Py：路径操作
来源：http://hz.jlsjyb.cn/gtoeqklxwk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.smart0.xyz/gtoeleofbk.html

[U25] Py：CSV 按字典读
来源：http://hz.meibo888.top/gtswrjvhmt.html

csv.DictReader(f)
来源：http://hz.gaohongyu789.top/gtbfkvcbvc.html

[U26] Py：并发下载
来源：http://hz.jqgfzy.top/gtmxluixhw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.wangdashe.top/gtayicpdjs.html

[U27] Py：异步 HTTP
来源：http://hz.chenzaomai.com/gtwoigvkji.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cqqwz.cn/gtvispmtfq.html

[U28] Py：类型别名
来源：http://hz.zdqjudy.top/gtomkxjslq.html

UserId = int
来源：http://hz.cucudq.cn/gtlubqymkg.html

[U29] Py：属性校验
来源：http://hz.pycfn.com/gtujlikpqz.html

@property 与 @x.setter 配合
来源：http://hz.yonumen.top/gtqlkieogm.html

[U30] Py：数据类
来源：http://hz.zhengqikj.top/gtuaskgzre.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gthgfrkzhc.html

[U31] Py：单测
来源：http://hz.ywan-chungtsiang.top/gtjmybjzoq.html

python -m pytest -q
来源：http://hz.gogol.net.cn/gtorrboulx.html

[U32] Py：代码格式化
来源：http://hz.0kj1m.cn/gttsnkwdel.html

ruff format . && ruff check --fix .
来源：http://hz.ivvv.top/gtzgvxpyme.html

[U33] Py：打包发布
来源：http://hz.jinyuanbaomall.cn/gtfxzjsqjj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xylfe.cn/gtfxfcrdfe.html

[U34] Py：判断编码
来源：http://hz.cqqwz.cn/gtbxxxrfhz.html

chardet.detect(raw)
来源：http://hz.wangshuangyany.cn/gtpitcvdlj.html

[U35] Py：发送邮件
来源：http://hz.hysaishi.cn/gtbiiavkwq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.pycfn.com/gtwkrhuwlx.html

[U36] Py：定时任务
来源：http://hz.shangyingyoupin.top/gtskwhkozd.html

schedule.every(10).minutes.do(job)
来源：http://hz.xuetiantiany.cn/gtxaacvjzx.html

[U37] Py：读写 Excel
来源：http://hz.hongshengwenyu.top/gtteptvyon.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nanxuanxn.top/gtskwuvrdd.html

[U38] Py：获取脚本所在目录
来源：http://hz.cheryme.top/gtntfgaxyo.html

Path(__file__).resolve().parent
来源：http://hz.bjfxy.top/gtqywhwcdw.html

[U39] Py：判断是否在交互环境
来源：http://hz.shanyushiyangkeji.top/gtxkzlcltg.html

sys.stdout.isatty()
来源：http://hz.nwbrower.top/gtojfflqzb.html

[U40] Py：打印到标准错误
来源：http://hz.sxryk.cn/gtnwckiwbn.html

print("err", file=sys.stderr)
来源：http://hz.wangshuangyany.cn/gtairqdrgu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zycfv.cn/gtgjirqkhy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hongshengwenyu.top/gtsuddtwuq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gotoacloud.top/gttqzjioud.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.birdmap.top/gtpluqreli.html

[U43] PHP：声明命名空间
来源：http://hz.nanxuanxn.top/gtzaymechg.html

namespace App\Http;
来源：http://hz.fengsongda.top/gtzufsvskm.html

[U44] PHP：开启严格类型
来源：http://hz.tanke756.top/gtvzczdeem.html

declare(strict_types=1);
来源：http://hz.zhixingplan.top/gtxxnfdobk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yonumen.top/gttartbpjd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gttzmxwwtr.html

[U46] PHP：可空类型
来源：http://hz.xinyue.icu/gtsvmylcim.html

?string $name = null
来源：http://hz.nwbrower.top/gtrisfpnth.html

[U47] PHP：联合类型
来源：http://hz.shuidangran.top/gtagcikizi.html

int|string $id
来源：http://hz.cashguo.top/gtkutbazwj.html

[U48] PHP：纯枚举
来源：http://hz.hfpthk.cn/gtcsqmbewl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.nanxinkj.top/gtwfggvmnt.html

[U49] PHP：只读属性
来源：http://hz.daria6918.cn/gtzliozpxd.html

public readonly string $name
来源：http://hz.hongshengwenyu.top/gtwusbemlf.html

[U50] PHP：构造器属性提升
来源：http://hz.jinghuilouyu.cn/gtgtevwzua.html

public function __construct(private int $id) {}
来源：http://hz.aibaodan.cn/gtpeqbobxo.html

[U51] PHP：数组解构
来源：http://hz.ydjk.org.cn/gtfqaumhvt.html

[$a, $b] = $arr;
来源：http://hz.ybcxt.top/gtscudrgez.html

[U52] PHP：箭头函数
来源：http://hz.chenjidiqi.icu/gtliivbobx.html

$double = fn($x) => $x * 2;
来源：http://hz.shanyushiyangkeji.top/gtuvykbhil.html

[U53] PHP：空合并运算符
来源：http://hz.yvedp.cn/gtugaqzakx.html

$v = $a ?? $b ?? "default";
来源：http://hz.xylfe.cn/gtkbmoofwh.html

[U54] PHP：空安全调用
来源：http://hz.hfpthk.cn/gtysetfdwi.html

$obj?->method()
来源：http://hz.cdnleiting.top/gtmbkonfrc.html

[U55] PHP：match 表达式
来源：http://hz.yj20258.top/gtwflegyyp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sufxvd.cn/gtmgzroqiz.html

[U56] PHP：命名参数
来源：http://hz.ybcxt.top/gthfttxtjd.html

f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtowbhbupp.html

[U57] PHP：字符串插值
来源：http://hz.haohaochexian.top/gtziwzpeso.html

"值: {$a}"
来源：http://hz.gogol.net.cn/gthvuszhtw.html

[U58] PHP：数组三件套
来源：http://hz.jqgufenzy.top/gtkkvwpuwr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hywenlv.cn/gtyegspgsy.html

[U59] PHP：自定义排序
来源：http://hz.ydjk.org.cn/gtuwlympqd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtcvegpect.html

[U60] PHP：JSON 编解码
来源：http://hz.ivvv.top/gtgtnapzbc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgfzy.top/gtmmkjfciq.html

[U61] PHP：正则
来源：http://hz.c1oappe.top/gthnztxpxb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gtubjrnvju.html

[U62] PHP：日期对象
来源：http://hz.aizwys.cn/gtzwnktdeq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.haohaochexian.top/gtqcxypftz.html

[U63] PHP：文件读写
来源：http://hz.shangyingyoupin.top/gtiapxrxrg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinghuilouyu.cn/gtbuwyzsou.html

[U64] PHP：目录遍历
来源：http://hz.redwolf501.top/gtlorxwcth.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhengqikj.top/gtavzvzczx.html

[U65] PHP：会话
来源：http://hz.hongshengwenyu.top/gttmsqmieu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.svipenyu.cn/gtkvtamejf.html

[U66] PHP：设置 Cookie
来源：http://hz.tianlin.xyz/gtrsdpprho.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zdqjudy.top/gttpfiwyxs.html

[U67] PHP：处理文件上传
来源：http://hz.iojbl.cn/gtnyjqtkuv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxinkj.top/gtpisfrilm.html

[U68] PHP：PDO 连接
来源：http://hz.jqgufenzy.top/gtkoqrpntq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.haohaochexian.top/gtwismccvy.html

[U69] PHP：PDO 预处理
来源：http://hz.smart0.xyz/gthasoobzg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yonumen.top/gtnkfuarby.html

[U70] PHP：PDO 事务
来源：http://hz.hysaishi.cn/gtktxhmoww.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yueranfly.top/gtledcechk.html

[U71] PHP：抛出异常
来源：http://hz.jyoumei.cn/gtxpwzuzxm.html

throw new RuntimeException("失败", 500);
来源：http://hz.tian-w.cn/gtorkbakuf.html

[U72] PHP：写错误日志
来源：http://hz.shzxlz.cn/gtsagkxuvg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.andypj.xyz/gtadxcjhgo.html

[U73] PHP：读取 ini 配置
来源：http://hz.yvedp.cn/gtnfptldio.html

parse_ini_file("config.ini", true)
来源：http://hz.jinghuilouyu.cn/gtnydahrft.html

[U74] PHP：读取环境变量
来源：http://hz.smart0.xyz/gtfcposwqx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.tian-w.cn/gtytvvjnbu.html

[U75] PHP：依赖注入
来源：http://hz.tian-w.cn/gttytzdlom.html

composer require psr/container
来源：http://hz.zhixingplan.top/gtyilumcco.html

[U76] PHP：简单路由
来源：http://hz.pycfn.com/gtamvnykyp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.andypj.xyz/gtuhnyuhxr.html

[U77] PHP：模板渲染
来源：http://hz.ehwqpu.com/gtmwncmrbt.html

composer require twig/twig
来源：http://hz.ydjk.org.cn/gttvwfxamm.html

[U78] PHP：单元测试
来源：http://hz.jyoumei.cn/gtvvrwgjnj.html

composer require --dev phpunit/phpunit
来源：http://hz.chenlongwang.top/gtpeffinhn.html

[U79] PHP：静态分析
来源：http://hz.dashuyun.cn/gtewyytjne.html

composer require --dev phpstan/phpstan
来源：http://hz.xinyue.icu/gtwpiusxoh.html

[U80] PHP：代码规范修复
来源：http://hz.wangdashe.top/gtzolzuzxg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yonumen.top/gtcrhozzbs.html

[U81] JS：初始化项目
来源：http://hz.shangyingyoupin.top/gtfnldeckj.html

npm init -y;  npm i express
来源：http://hz.kuanghao11.cn/gtcqogmfdi.html

[U82] JS：package.json 脚本
来源：http://hz.jqgufenzy.top/gtsumwlhps.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinghuilouyu.cn/gtokacvkon.html

[U83] JS：ES Module 导入导出
来源：http://hz.hysaishi.cn/gtoqzdztdf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hysaishi.cn/gtwprcrklc.html

[U84] JS：CommonJS 写法
来源：http://hz.cucudq.cn/gtqoxxqeml.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.mhx1999.top/gtbiobfdzr.html

[U85] JS：可选链
来源：http://hz.hysaishi.cn/gtfmebkutl.html

a?.b?.c
来源：http://hz.guowangkeji.top/gtpnvejmev.html

[U86] JS：空值合并
来源：http://hz.yuanzhike.top/gtlvxjlzch.html

a ?? b
来源：http://hz.quarkkingdee.top/gtuuskjrrf.html

[U87] JS：解构默认值
来源：http://hz.meibo888.top/gtyhobbdhl.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xuanzx.com/gtlszrkekx.html

[U88] JS：对象展开合并
来源：http://hz.yonumen.top/gtrejfbwpy.html

{ ...a, ...b }
来源：http://hz.redwolf501.top/gttbxpzuus.html

[U89] JS：数组去重
来源：http://hz.yonumen.top/gtamuqcses.html

[...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtitaeoccc.html

[U90] JS：数字数组排序
来源：http://hz.shzxlz.cn/gtflnfcznz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtycogdybz.html

[U91] JS：对象键值遍历
来源：http://hz.ybcxt.top/gttjtwzjsx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinyuanbaomall.cn/gtbebppwlp.html

[U92] JS：深拷贝
来源：http://hz.yueranfly.top/gtisbkrlgn.html

structuredClone(obj)
来源：http://hz.cdnleiting.top/gtiqqtkxat.html

[U93] JS：模板字符串
来源：http://hz.jqgufenzy.top/gtdaejrpwq.html

`共 ${n} 条`
来源：http://hz.jqgfzy.top/gtnnqntgwe.html

[U94] JS：箭头函数
来源：http://hz.gogol.net.cn/gtauxlaxoi.html

const double = x => x * 2;
来源：http://hz.zhaomingkeji.xyz/gtyagzmtyh.html

[U95] JS：Promise 包装
来源：http://hz.jiagoushi.top/gtyaotqdvk.html

new Promise((resolve, reject) => {})
来源：http://hz.fengsongda.top/gtfmngbgos.html

[U96] JS：async/await 与异常
来源：http://hz.sxryk.cn/gtwrcevojz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtyjxcxruv.html

[U97] JS：并发请求
来源：http://hz.yanxiufei.cn/gtcuvxnvkr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtfakssugq.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhixingplan.top/gtxjzoityo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.fzhhl.top/gtcrwoseks.html

[U99] JS：事件监听
来源：http://hz.zhixingplan.top/gtrphdxvfs.html

el.addEventListener("click", e => {})
来源：http://hz.hnxiangtu.top/gtmbpwfbmr.html

[U100] JS：DOM 查询
来源：http://hz.hnqzz.top/gtmwjlkvpj.html

document.querySelector(".item")
来源：http://hz.birdmap.top/gtsbnccfif.html

[U101] JS：classList 操作
来源：http://hz.hammf.cn/gtmxfpctsc.html

el.classList.toggle("active")
来源：http://hz.nwbrower.top/gtcwhaatrm.html

[U102] JS：本地存储
来源：http://hz.gzhubu.top/gtnxiqmxzm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinqigfzy.top/gtyonbbajn.html

[U103] JS：定时器
来源：http://hz.zhixingplan.top/gtumkivbqj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj202588.top/gtaeonntca.html

[U104] JS：防抖
来源：http://hz.shanyushiyangtech.top/gtteatiept.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtkepagexf.html

[U105] JS：节流
来源：http://hz.gotoacloud.top/gtskqvgfdo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.sysykeji.top/gtnjgwbazz.html

[U106] JS：日期格式化
来源：http://hz.jqgufenzy.top/gtipduhlpq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tianlin.xyz/gthdavsjeb.html

[U107] JS：数字千分位
来源：http://hz.daria6918.cn/gtlxadedsz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gaohongyu789.top/gtlhtiaswe.html

[U108] JS：随机整数
来源：http://hz.chenjidiqi.icu/gtaapwbudl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.kuanghao11.cn/gtxzbmissk.html

[U109] JS：数组分组
来源：http://hz.havefunace.top/gtphktalgf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xuetiantiany.cn/gtvqxokgpa.html

[U110] JS：数组分块
来源：http://hz.jinqigfzy.top/gtmwtjjdyh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.daria6918.cn/gtkzrxywqe.html

[U111] JS：对象转 Map
来源：http://hz.aibaodan.cn/gtmrdszfjk.html

new Map(Object.entries(obj))
来源：http://hz.nwbrower.top/gtjqifvbyg.html

[U112] JS：字符串补位
来源：http://hz.daxiang520.top/gtdrutledn.html

"7".padStart(3, "0")
来源：http://hz.jqgufenzy.top/gtxwvdymlx.html

[U113] JS：正则替换全部
来源：http://hz.chenlongwang.top/gtowgwxmqi.html

s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtijvljucg.html

[U114] JS：JSON 深比较
来源：http://hz.ydzc1.top/gtxrgbgnfs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yangfankeji.com/gtsorlietv.html

[U115] JS：生成 UUID
来源：http://hz.yj202588.top/gtwmlwspto.html

crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtbjzxgpwh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guannengcc.top/gtjgysaqau.html

/** @param {string} name */ function f(name) {}
来源：http://hz.guannengcc.top/gtfejbynsc.html

[U117] JS：单元测试
来源：http://hz.haohaochexian.top/gtuugdwfth.html

npm i -D vitest;  npx vitest
来源：http://hz.jianghu66.top/gtrfovzmmv.html

[U118] JS：开发服务器
来源：http://hz.smart0.xyz/gtkvalvjws.html

npm i -D vite;  npx vite
来源：http://hz.cqqwz.cn/gtmwxxncxe.html

[U119] JS：生产构建
来源：http://hz.sxryk.cn/gttfrmmyrq.html

npx vite build
来源：http://hz.hfpthk.cn/gtnvzgbjyz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.haohaochexian.top/gtmezcamlw.html

import.meta.env.VITE_API_URL
来源：http://hz.sxryk.cn/gtdirxbqqx.html

================================================================================
来源：http://hz.cqqwz.cn/gtpnkuhtyy.html

统计汇总
来源：http://hz.yj20258888.top/gtntsupqix.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtvgathkou.html

按语言统计（条）：
来源：http://hz.zhixingplan.top/gtfuxwvqnn.html

Python ......... 252
来源：http://hz.jinqigufen.top/gtyfgmhwrc.html

PHP ............ 252
来源：http://hz.cucudq.cn/gtbwjgbdem.html

JavaScript ..... 252
来源：http://hz.yonumen.top/gtfygjefht.html

TypeScript ..... 212
来源：http://hz.haohaochexian.top/gtinxdjgcx.html

Java ........... 212
来源：http://hz.zhijiandao.cn/gtubqxgrpf.html

Go ............. 212
来源：http://hz.cheryme.top/gtbmydcckb.html

Ruby ........... 212
来源：http://hz.ywan-chungtsiang.top/gthqvozdis.html

C# ............. 212
来源：http://hz.guannengcc.top/gtkqqcsgdd.html

C .............. 30
来源：http://hz.52xcode.cn/gtqxgveerk.html

C++ ............ 30
来源：http://hz.hfpthk.cn/gtyecxiejs.html

SQL ............ 90
来源：http://hz.chenzaomai.com/gtttuhaiqy.html

Bash ........... 80
来源：http://hz.shuidangran.top/gtsejtdbry.html

Kotlin ......... 15
来源：http://hz.gzhubu.top/gtqfwieelv.html

Swift .......... 15
来源：http://hz.fzhhl.top/gthxpgaspz.html

Lua ............ 10
来源：http://hz.9152youxi.cn/gtpcbbbgor.html

Perl ........... 10
来源：http://hz.ydzc1.top/gtnavstbzy.html

Scala .......... 10
来源：http://hz.cheryme.top/gtshupbyzs.html

------------------------------------
来源：http://hz.kuanghao11.cn/gtxukbgxzi.html

合计 ........... 2106 条
来源：http://hz.andypj.xyz/gthuivgjhr.html

按章节统计：
来源：http://hz.cashguo.top/gtaapzlcxt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhiwuduotai.top/gtvghvclzc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangkeji.top/gtordlxfxl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtefumuzab.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pengpengdd.cyou/gtzmvtzolj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yanxiufei.cn/gtajrevnxs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jqgufenzy.top/gtuhqdkaoh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtiibvbvxe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhoulong.xyz/gtjvoevzfh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtfdcxhxri.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gotoacloud.top/gtlqlhkonk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtjwrgtbmo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtoslsceqt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gtgdkvgqmf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.pycfn.com/gterhqrite.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuanzx.com/gtpavhzxtg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtxwwswaqt.html

Q SQL 专题                              90
来源：http://hz.jinqigufen.top/gtrptrdawn.html

R Bash 专题                             80
来源：http://hz.zhijiandao.cn/gtrgnlqjax.html

S C / C++ 专题                          60
来源：http://hz.zhengqikj.top/gtbhvxtqhm.html

T 其他语言补充                          60
来源：http://hz.ywan-chungtsiang.top/gtkysjenba.html


<!-- 参考信息 -->