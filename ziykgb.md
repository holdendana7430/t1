代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhixingplan.top/gtnruwzcqb.html

[T55] Scala：集合过滤
来源：http://hz.pengpengdd.cyou/gtcdvxrupy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yuanzhike.top/gtwmzmqzoc.html

[T56] Scala：样例类
来源：http://hz.yonumen.top/gtyqdgwfbk.html

case class User(name: String, age: Int)
来源：http://hz.jinqigfzy.top/gtqcnsioav.html

[T57] Scala：模式匹配
来源：http://hz.zhengqikj.top/gtqasimjjp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.9152youxi.cn/gtjeraxqee.html

[T58] Scala：函数定义
来源：http://hz.zhoulong.xyz/gtahiwoaxk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jianghu66.top/gtuqaezumh.html

[T59] Scala：循环
来源：http://hz.zhijiandao.cn/gtcxqvzuvv.html

for (i <- 1 to 10) println(i)
来源：http://hz.hammf.cn/gtibyainpl.html

[T60] Scala：折叠
来源：http://hz.zhongyouzk.top/gtboxsyonb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yongpay.top/gtjhruiucm.html

================================================================================
来源：http://hz.hywenlv.cn/gtbblmuhoz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.pengpengdd.cyou/gtxweuhxgt.html

================================================================================
来源：http://hz.havefunace.top/gtiytvrzzf.html

[U01] Py：创建虚拟环境
来源：http://hz.c1oappe.top/gtknewfbeq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.haohaochexian.top/gtydvwjfff.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nwbrower.top/gtdezxsvph.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj202588.top/gtfbjkucsd.html

[U03] Py：加载 .env 配置
来源：http://hz.kuanghao11.cn/gtmkbnorhe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xinyue.icu/gthlyifvjc.html

[U04] Py：变量调试打印
来源：http://hz.daxiang520.top/gttednorbt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinqigfzy.top/gtlfoznfqf.html

[U05] Py：列表去重且保序
来源：http://hz.yanxiufei.cn/gtihgkcilg.html

list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtbptqpicn.html

[U06] Py：合并两个字典
来源：http://hz.hongshengwenyu.top/gtkmjbsawh.html

{**a, **b}
来源：http://hz.sufxvd.cn/gtwqlefunn.html

[U07] Py：反转字典键值
来源：http://hz.gotoacloud.top/gtwbzunixo.html

{v: k for k, v in d.items()}
来源：http://hz.cheryme.top/gtcuoviimg.html

[U08] Py：展平二维列表
来源：http://hz.ydzc1.top/gtmdkcefrk.html

[y for x in nested for y in x]
来源：http://hz.cdnleiting.top/gtwuktscbn.html

[U09] Py：字典取最大值的键
来源：http://hz.zdqjudy.top/gthtzmkrec.html

max(d, key=d.get)
来源：http://hz.tian-w.cn/gtgxravtyz.html

[U10] Py：按值排序字典
来源：http://hz.316326.xyz/gtgzqmeavg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gzhubu.top/gtwgugidik.html

[U11] Py：生成器表达式
来源：http://hz.chenjidiqi.icu/gtbmbofjqj.html

(x * 2 for x in arr)
来源：http://hz.cucudq.cn/gtisuoogcj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.wangdashe.top/gtgjvewazj.html

Counter(arr).most_common(3)
来源：http://hz.sxryk.cn/gthregdbpw.html

[U13] Py：固定长度队列
来源：http://hz.snrcjt.cn/gttkkyolsg.html

deque(maxlen=10)
来源：http://hz.cucudq.cn/gtcfxbvvpp.html

[U14] Py：分组收集到列表
来源：http://hz.gogol.net.cn/gtkipezeqn.html

defaultdict(list)
来源：http://hz.chenzaomai.com/gtfdzcoqxk.html

[U15] Py：高精度计时
来源：http://hz.jiagoushi.top/gtdariqtjk.html

t = time.perf_counter()
来源：http://hz.nwbrower.top/gtummhlzkt.html

[U16] Py：命令行参数解析
来源：http://hz.ydjk.org.cn/gtoafeizjx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhixingplan.top/gtxnvwbmgs.html

[U17] Py：初始化日志
来源：http://hz.chenzaomai.com/gtximraxkz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangdashe.top/gtebphhzqi.html

[U18] Py：预编译正则
来源：http://hz.nanxinkj.top/gtlenabhff.html

pat = re.compile(r"\d+")
来源：http://hz.feifeiyinyue.top/gtaiyvfdqv.html

[U19] Py：正则替换带回调
来源：http://hz.jqgufenzy.top/gtwgsffswp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj20258.top/gtlquumzie.html

[U20] Py：缓存函数结果
来源：http://hz.chenjidiqi.icu/gtmiftdbnr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.fengsongda.top/gtrqangsgx.html

[U21] Py：自定义上下文管理器
来源：http://hz.jqgufenzy.top/gtsppgfyxz.html

@contextlib.contextmanager
来源：http://hz.andypj.xyz/gtvucryxku.html

[U22] Py：矩阵转置
来源：http://hz.meibo888.top/gtcnwoqmpi.html

list(zip(*m))
来源：http://hz.316326.xyz/gtcuphnmmr.html

[U23] Py：分块读取大文件
来源：http://hz.yuxming.cn/gtduqpznhq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yangfankeji.com/gtpgryeyap.html

[U24] Py：路径操作
来源：http://hz.bjfxy.top/gtpygbxray.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj20258888.top/gtrwnkveqi.html

[U25] Py：CSV 按字典读
来源：http://hz.cheryme.top/gtajzgbket.html

csv.DictReader(f)
来源：http://hz.daxiang520.top/gtykhmlbuw.html

[U26] Py：并发下载
来源：http://hz.yj202588.top/gtlmyfbomh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yj20258.top/gtdbumfybr.html

[U27] Py：异步 HTTP
来源：http://hz.kuanghao11.cn/gtovlkegbm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gzhubu.top/gtxpdasipl.html

[U28] Py：类型别名
来源：http://hz.jianghu66.top/gtmmlfjzyo.html

UserId = int
来源：http://hz.ivvv.top/gtwpqecwso.html

[U29] Py：属性校验
来源：http://hz.xziqi.cn/gtcoijqvvt.html

@property 与 @x.setter 配合
来源：http://hz.nwbrower.top/gtrvopmtbi.html

[U30] Py：数据类
来源：http://hz.ybcxt.top/gteslyggpo.html

@dataclass(slots=True)
来源：http://hz.aibaodan.cn/gtrbfcnctv.html

[U31] Py：单测
来源：http://hz.yanxiufei.cn/gtoolfjkgt.html

python -m pytest -q
来源：http://hz.chenzaomai.com/gtbeqztigv.html

[U32] Py：代码格式化
来源：http://hz.zhaomingkeji.xyz/gtzdybbfyo.html

ruff format . && ruff check --fix .
来源：http://hz.vqdsnc.cn/gthyxzqbit.html

[U33] Py：打包发布
来源：http://hz.tanke756.top/gtibypgxzi.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ivvv.top/gtuvhlucmy.html

[U34] Py：判断编码
来源：http://hz.0kj1m.cn/gtfdwoxbwi.html

chardet.detect(raw)
来源：http://hz.tianlin.xyz/gtuehbpzcj.html

[U35] Py：发送邮件
来源：http://hz.svipenyu.cn/gtiaqyxdmb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.quarkkingdee.top/gtwfetzhwd.html

[U36] Py：定时任务
来源：http://hz.ehwqpu.com/gtdblcbapg.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj202588.top/gtsckhzqmy.html

[U37] Py：读写 Excel
来源：http://hz.fengsongda.top/gtqzvnbgnx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hammf.cn/gtazlvnyxh.html

[U38] Py：获取脚本所在目录
来源：http://hz.aibaodan.cn/gtchinxpev.html

Path(__file__).resolve().parent
来源：http://hz.sweek.top/gtjhistioi.html

[U39] Py：判断是否在交互环境
来源：http://hz.dianchejie.cn/gtccajknca.html

sys.stdout.isatty()
来源：http://hz.zhijiandao.cn/gtbpxfjtcf.html

[U40] Py：打印到标准错误
来源：http://hz.xuanzx.com/gtcmodlybp.html

print("err", file=sys.stderr)
来源：http://hz.shuidangran.top/gtsitkmhci.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sweek.top/gtajzknfqp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.iojbl.cn/gtwwfstiym.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hnxiangtu.top/gtxlgayyyw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.smart0.xyz/gtmjttpdol.html

[U43] PHP：声明命名空间
来源：http://hz.yonumen.top/gtjmmcjzrx.html

namespace App\Http;
来源：http://hz.havefunace.top/gtcwhakxhz.html

[U44] PHP：开启严格类型
来源：http://hz.sufxvd.cn/gtdflklfuu.html

declare(strict_types=1);
来源：http://hz.c1oappe.top/gtxkdbjhvp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jqgufenzy.top/gtboyheyiv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtoozcalpf.html

[U46] PHP：可空类型
来源：http://hz.0kj1m.cn/gtdvizsous.html

?string $name = null
来源：http://hz.yueranfly.top/gtntwhyvsu.html

[U47] PHP：联合类型
来源：http://hz.c1oappe.top/gtoeqtoyll.html

int|string $id
来源：http://hz.jlsjyb.cn/gtebufoafx.html

[U48] PHP：纯枚举
来源：http://hz.gogol.net.cn/gtsvldxxyy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shuidangran.top/gtzlgddsxk.html

[U49] PHP：只读属性
来源：http://hz.jinghuilouyu.cn/gtmyuvbwxm.html

public readonly string $name
来源：http://hz.wangdashe.top/gtjewfikjp.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258.top/gtbyljmevw.html

public function __construct(private int $id) {}
来源：http://hz.daxiang520.top/gtuydflhkg.html

[U51] PHP：数组解构
来源：http://hz.hongshengwenyu.top/gtyppcgokj.html

[$a, $b] = $arr;
来源：http://hz.chenzaomai.com/gtvhmnuysi.html

[U52] PHP：箭头函数
来源：http://hz.jlsjyb.cn/gtkhurwplk.html

$double = fn($x) => $x * 2;
来源：http://hz.jinqigfzy.top/gtlnxenwnj.html

[U53] PHP：空合并运算符
来源：http://hz.hfpthk.cn/gtrgescirr.html

$v = $a ?? $b ?? "default";
来源：http://hz.ywan-chungtsiang.top/gtjzydbgbz.html

[U54] PHP：空安全调用
来源：http://hz.yongpay.top/gtsivhyvwl.html

$obj?->method()
来源：http://hz.yvedp.cn/gtdojqfkev.html

[U55] PHP：match 表达式
来源：http://hz.hammf.cn/gtvbhlsbpe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shanyushiyangtech.top/gtdwqhycrd.html

[U56] PHP：命名参数
来源：http://hz.xziqi.cn/gttsocpzds.html

f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtqkxfbjoa.html

[U57] PHP：字符串插值
来源：http://hz.daria6918.cn/gtalhkgjzt.html

"值: {$a}"
来源：http://hz.nanxuanxn.top/gteofjsyah.html

[U58] PHP：数组三件套
来源：http://hz.gogol.net.cn/gtuvhpivup.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sweek.top/gtnmsjdxqp.html

[U59] PHP：自定义排序
来源：http://hz.aizwys.cn/gtyvrhofps.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenlongwang.top/gtzjoqwlgb.html

[U60] PHP：JSON 编解码
来源：http://hz.gzhubu.top/gtgvbmqvjp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shanyushiyangtech.top/gtxfwfzijj.html

[U61] PHP：正则
来源：http://hz.sufxvd.cn/gtaexqfmis.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtopemjoyu.html

[U62] PHP：日期对象
来源：http://hz.sufxvd.cn/gtcpdmjmfk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hywenlv.cn/gtwnddadhy.html

[U63] PHP：文件读写
来源：http://hz.yj20258888.top/gtnewjmnru.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhoulong.xyz/gtkuywhubu.html

[U64] PHP：目录遍历
来源：http://hz.chenjidiqi.icu/gtkkovkaas.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sysykeji.top/gtpsloizzf.html

[U65] PHP：会话
来源：http://hz.zhiwuduotai.top/gtuqcwihwb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zdqjudy.top/gtsjjqtxku.html

[U66] PHP：设置 Cookie
来源：http://hz.yonumen.top/gthulqiufr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.snrcjt.cn/gtxavtclic.html

[U67] PHP：处理文件上传
来源：http://hz.shzxlz.cn/gtfnhrpotr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zdqjudy.top/gtfjmkgmnd.html

[U68] PHP：PDO 连接
来源：http://hz.chenlongwang.top/gtjdejbwlv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.birdmap.top/gtxukgmmmg.html

[U69] PHP：PDO 预处理
来源：http://hz.andypj.xyz/gtdbatewux.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shuidangran.top/gtqftvytze.html

[U70] PHP：PDO 事务
来源：http://hz.zycfv.cn/gtcjqauzsq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yj20258888.top/gtgtfdjzpj.html

[U71] PHP：抛出异常
来源：http://hz.52xcode.cn/gtfoifhdbu.html

throw new RuntimeException("失败", 500);
来源：http://hz.bjfxy.top/gtbjdtxpbo.html

[U72] PHP：写错误日志
来源：http://hz.pengpengdd.cyou/gtvhmaeyzv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.daria6918.cn/gtxniyekdh.html

[U73] PHP：读取 ini 配置
来源：http://hz.0kj1m.cn/gtnuttyixc.html

parse_ini_file("config.ini", true)
来源：http://hz.yongpay.top/gtzpcfkbks.html

[U74] PHP：读取环境变量
来源：http://hz.feifeiyinyue.top/gtgcktsfcs.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sysykeji.top/gtcxtqucfv.html

[U75] PHP：依赖注入
来源：http://hz.chenzaomai.com/gtwqveegwt.html

composer require psr/container
来源：http://hz.yueranfly.top/gtaibbrzmz.html

[U76] PHP：简单路由
来源：http://hz.yanxiufei.cn/gtcwmtsrxp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.kuanghao11.cn/gtxbcehnqg.html

[U77] PHP：模板渲染
来源：http://hz.hysaishi.cn/gtjojpeeyy.html

composer require twig/twig
来源：http://hz.ywan-chungtsiang.top/gtbwlulelh.html

[U78] PHP：单元测试
来源：http://hz.chenlongwang.top/gtsewhtlvs.html

composer require --dev phpunit/phpunit
来源：http://hz.cdnleiting.top/gtlwhbixzp.html

[U79] PHP：静态分析
来源：http://hz.gzhubu.top/gtknindfwb.html

composer require --dev phpstan/phpstan
来源：http://hz.ppjwa.cn/gtdohbarmf.html

[U80] PHP：代码规范修复
来源：http://hz.yuanzhike.top/gtcepothvs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.gogol.net.cn/gtnlkfkybp.html

[U81] JS：初始化项目
来源：http://hz.cqqwz.cn/gtcbbrzbzw.html

npm init -y;  npm i express
来源：http://hz.guowangkeji.top/gtdteawcxq.html

[U82] JS：package.json 脚本
来源：http://hz.yj202588.top/gtjzlobkam.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.meibo888.top/gtnhnxnvbz.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhoulong.xyz/gtkgzhrfio.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.dianchejie.cn/gtricwryoi.html

[U84] JS：CommonJS 写法
来源：http://hz.yvedp.cn/gtjhkgcihg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cqqwz.cn/gtmdwsfoya.html

[U85] JS：可选链
来源：http://hz.xziqi.cn/gtexhgatud.html

a?.b?.c
来源：http://hz.bjfxy.top/gtlgyoebhz.html

[U86] JS：空值合并
来源：http://hz.cqqwz.cn/gthcpepjbv.html

a ?? b
来源：http://hz.jinqigfzy.top/gtlsmnzbzn.html

[U87] JS：解构默认值
来源：http://hz.ehwqpu.com/gtrekbqqqj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yongpay.top/gtitqzgkad.html

[U88] JS：对象展开合并
来源：http://hz.tian-w.cn/gtkvzosgtq.html

{ ...a, ...b }
来源：http://hz.hnqzz.top/gthtkxnzol.html

[U89] JS：数组去重
来源：http://hz.hnxiangtu.top/gtguwggwll.html

[...new Set(arr)]
来源：http://hz.xziqi.cn/gtcoiuwxrc.html

[U90] JS：数字数组排序
来源：http://hz.chenzaomai.com/gtshkebjnr.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtgzrdjtzx.html

[U91] JS：对象键值遍历
来源：http://hz.ehwqpu.com/gtlhgsrofu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhaomingkeji.xyz/gtfijhdika.html

[U92] JS：深拷贝
来源：http://hz.daxiang520.top/gtxcljqcnt.html

structuredClone(obj)
来源：http://hz.cucudq.cn/gtgbpgiham.html

[U93] JS：模板字符串
来源：http://hz.hongshengwenyu.top/gtwkxyjjmb.html

`共 ${n} 条`
来源：http://hz.yuxming.cn/gtxromgdbd.html

[U94] JS：箭头函数
来源：http://hz.zhijiandao.cn/gtqrjygiis.html

const double = x => x * 2;
来源：http://hz.xuetiantiany.cn/gtwzqwlkdn.html

[U95] JS：Promise 包装
来源：http://hz.ivvv.top/gthozoeehv.html

new Promise((resolve, reject) => {})
来源：http://hz.shangyingyoupin.top/gtuzphhozz.html

[U96] JS：async/await 与异常
来源：http://hz.nwbrower.top/gtxnffsupv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gtndwrwwyy.html

[U97] JS：并发请求
来源：http://hz.wangshuangyany.cn/gtfdnnrxfw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtapwbsbfd.html

[U98] JS：fetch 带 JSON
来源：http://hz.jyoumei.cn/gtzgdscjoe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.cheryme.top/gtpjmqjyrn.html

[U99] JS：事件监听
来源：http://hz.smart0.xyz/gtflehdwve.html

el.addEventListener("click", e => {})
来源：http://hz.jyoumei.cn/gtthdtnvbm.html

[U100] JS：DOM 查询
来源：http://hz.guowangkeji.top/gtwpdquwtd.html

document.querySelector(".item")
来源：http://hz.shanyushiyangtech.top/gtujmadhhg.html

[U101] JS：classList 操作
来源：http://hz.xuetiantiany.cn/gtxeqfjssm.html

el.classList.toggle("active")
来源：http://hz.yonumen.top/gtwjvwihke.html

[U102] JS：本地存储
来源：http://hz.zycfv.cn/gttzvvwggx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhongyouzk.top/gtoelbtxca.html

[U103] JS：定时器
来源：http://hz.gogol.net.cn/gtgnrrqtxb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ywan-chungtsiang.top/gtoexmizfq.html

[U104] JS：防抖
来源：http://hz.hysaishi.cn/gtzozhmemf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtwujigpyw.html

[U105] JS：节流
来源：http://hz.zhixingplan.top/gtbswrjnwe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xinyue.icu/gtjesmuyja.html

[U106] JS：日期格式化
来源：http://hz.pycfn.com/gtrqixcoyb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.haohaochexian.top/gtylzncqsj.html

[U107] JS：数字千分位
来源：http://hz.guannengcc.top/gttekobvnr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.smart0.xyz/gtgcpybitv.html

[U108] JS：随机整数
来源：http://hz.0kj1m.cn/gtxmnzyzqs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinqigufen.top/gtlmyhjdiv.html

[U109] JS：数组分组
来源：http://hz.316326.xyz/gtksnnuyzs.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cucudq.cn/gtrdthhnbx.html

[U110] JS：数组分块
来源：http://hz.yvedp.cn/gttabwppxg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinqigufen.top/gtpcnntyrz.html

[U111] JS：对象转 Map
来源：http://hz.birdmap.top/gtzonmivnl.html

new Map(Object.entries(obj))
来源：http://hz.jianghu66.top/gtcibtifbc.html

[U112] JS：字符串补位
来源：http://hz.gotoacloud.top/gtglbwohse.html

"7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtgnrhpnbl.html

[U113] JS：正则替换全部
来源：http://hz.xingfuxueyuan.xyz/gtaiennfgi.html

s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtjjeigbex.html

[U114] JS：JSON 深比较
来源：http://hz.wangshuangyany.cn/gtnxgadvbk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtbqyoqnvg.html

[U115] JS：生成 UUID
来源：http://hz.hysaishi.cn/gtjykhaprc.html

crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtbuldhbsa.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pengpengdd.cyou/gtlainkhly.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sxryk.cn/gtscmjspsj.html

[U117] JS：单元测试
来源：http://hz.gaohongyu789.top/gtjmccgciz.html

npm i -D vitest;  npx vitest
来源：http://hz.quarkkingdee.top/gtgidfxylh.html

[U118] JS：开发服务器
来源：http://hz.jiagoushi.top/gtqjdzxiec.html

npm i -D vite;  npx vite
来源：http://hz.0kj1m.cn/gtpkurbate.html

[U119] JS：生产构建
来源：http://hz.iojbl.cn/gthytxrxdv.html

npx vite build
来源：http://hz.zhengqikj.top/gtboorijip.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yueranfly.top/gtyjwwwclz.html

import.meta.env.VITE_API_URL
来源：http://hz.wangshuangyany.cn/gtloqimogn.html

================================================================================
来源：http://hz.zhixingplan.top/gtwhndtdru.html

统计汇总
来源：http://hz.nanxinkj.top/gtkfdvrcme.html

================================================================================
来源：http://hz.bjfxy.top/gtqyppdlbi.html

按语言统计（条）：
来源：http://hz.tian-w.cn/gtmgpfxkgk.html

Python ......... 252
来源：http://hz.yangfankeji.com/gttzrmgnvs.html

PHP ............ 252
来源：http://hz.fengsongda.top/gtzqgsrwmb.html

JavaScript ..... 252
来源：http://hz.cucudq.cn/gthnlzkkzh.html

TypeScript ..... 212
来源：http://hz.daria6918.cn/gtydrkqskl.html

Java ........... 212
来源：http://hz.xziqi.cn/gtpqdzddtt.html

Go ............. 212
来源：http://hz.fzhhl.top/gtcpelpgow.html

Ruby ........... 212
来源：http://hz.redwolf501.top/gtawxgnfhx.html

C# ............. 212
来源：http://hz.sweek.top/gtpvbrsnze.html

C .............. 30
来源：http://hz.jqgfzy.top/gtaksdzmhx.html

C++ ............ 30
来源：http://hz.birdmap.top/gtwtymyqkk.html

SQL ............ 90
来源：http://hz.cashguo.top/gtsoyuauuf.html

Bash ........... 80
来源：http://hz.haohaochexian.top/gtzfinkgto.html

Kotlin ......... 15
来源：http://hz.shanyushiyangtech.top/gtbjbgvqof.html

Swift .......... 15
来源：http://hz.svipenyu.cn/gtxrhgygxk.html

Lua ............ 10
来源：http://hz.wangshuangyany.cn/gtrfxjpzvu.html

Perl ........... 10
来源：http://hz.hfpthk.cn/gtskulesuh.html

Scala .......... 10
来源：http://hz.zhongyouzk.top/gtehunhjlc.html

------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtxkbusccp.html

合计 ........... 2106 条
来源：http://hz.sweek.top/gthpbsouhc.html

按章节统计：
来源：http://hz.bjfxy.top/gtyxdrbhks.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhengqikj.top/gttkxtndui.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangtech.top/gtlwxsxwub.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shangyingyoupin.top/gtlbwgfpox.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtzcfhkahq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.bjfxy.top/gtxnftwhrq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.dashuyun.cn/gtvwkbqggh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cucudq.cn/gtafcqclmm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xingfuxueyuan.xyz/gtlpeypkbv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtppavnunl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hysaishi.cn/gtgrwfhilh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtasotrubw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gthncqysyh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtjfikgoea.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zdqjudy.top/gtnkoclulk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.aibaodan.cn/gtzccptmpu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtpwxkmixf.html

Q SQL 专题                              90
来源：http://hz.snrcjt.cn/gtihtfqmvd.html

R Bash 专题                             80
来源：http://hz.hfpthk.cn/gtavoephux.html

S C / C++ 专题                          60
来源：http://hz.hammf.cn/gtbydcqxrx.html

T 其他语言补充                          60
来源：http://hz.yangfankeji.com/gtsuldwolu.html


<!-- 参考信息 -->