代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.0kj1m.cn/gtcnoojzwd.html

[T55] Scala：集合过滤
来源：http://hz.0kj1m.cn/gtluvdhiol.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hfpthk.cn/gtpwtluvcf.html

[T56] Scala：样例类
来源：http://hz.yonumen.top/gtlmwbrane.html

case class User(name: String, age: Int)
来源：http://hz.guowangkeji.top/gtzyvzfqjg.html

[T57] Scala：模式匹配
来源：http://hz.hysaishi.cn/gtxkskcpzt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxinkj.top/gtnznngazd.html

[T58] Scala：函数定义
来源：http://hz.havefunace.top/gtqlfgryoh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgufenzy.top/gtxzhzishz.html

[T59] Scala：循环
来源：http://hz.hongshengwenyu.top/gtzurlvjcb.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuetiantiany.cn/gtbvlrtmha.html

[T60] Scala：折叠
来源：http://hz.zhengqikj.top/gtlwsfbcwo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydjk.org.cn/gtbpcdgzce.html

================================================================================
来源：http://hz.jinqigufen.top/gtqiisfemp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuxming.cn/gtdyvpgitd.html

================================================================================
来源：http://hz.iojbl.cn/gtvixccxmf.html

[U01] Py：创建虚拟环境
来源：http://hz.shzxlz.cn/gtequsfbub.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jiagoushi.top/gtyvjfuddy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fengsongda.top/gtkqquydnz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yongpay.top/gtbkxzsekn.html

[U03] Py：加载 .env 配置
来源：http://hz.zhongyouzk.top/gtbthtrlzh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shangyingyoupin.top/gtjeaqwguw.html

[U04] Py：变量调试打印
来源：http://hz.yj202588.top/gtlxqsygui.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xuetiantiany.cn/gtszrgmnji.html

[U05] Py：列表去重且保序
来源：http://hz.quarkkingdee.top/gtlwmqscjl.html

list(dict.fromkeys(arr))
来源：http://hz.yj202588.top/gtzrfwcweq.html

[U06] Py：合并两个字典
来源：http://hz.zhongyouzk.top/gtqzcfrvfo.html

{**a, **b}
来源：http://hz.shangyingyoupin.top/gtxubjdtzv.html

[U07] Py：反转字典键值
来源：http://hz.zhaomingkeji.xyz/gtcwbandcr.html

{v: k for k, v in d.items()}
来源：http://hz.xuanzx.com/gtvpfkqzct.html

[U08] Py：展平二维列表
来源：http://hz.cqqwz.cn/gtfbymoowj.html

[y for x in nested for y in x]
来源：http://hz.nwbrower.top/gtzoyvmyzo.html

[U09] Py：字典取最大值的键
来源：http://hz.wangshuangyany.cn/gtuynbfqli.html

max(d, key=d.get)
来源：http://hz.yvedp.cn/gttnvwgoxw.html

[U10] Py：按值排序字典
来源：http://hz.pycfn.com/gtfhxfvkgm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ehwqpu.com/gtajbafuea.html

[U11] Py：生成器表达式
来源：http://hz.sxryk.cn/gtpmrlxbea.html

(x * 2 for x in arr)
来源：http://hz.ppjwa.cn/gtkifftafb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.kuanghao11.cn/gtzeyeqxkq.html

Counter(arr).most_common(3)
来源：http://hz.ydjk.org.cn/gtsujzrjne.html

[U13] Py：固定长度队列
来源：http://hz.fengsongda.top/gtflqtticd.html

deque(maxlen=10)
来源：http://hz.zhaomingkeji.xyz/gthknyztih.html

[U14] Py：分组收集到列表
来源：http://hz.svipenyu.cn/gtitnhrrlt.html

defaultdict(list)
来源：http://hz.jinqigfzy.top/gtyvxnahkp.html

[U15] Py：高精度计时
来源：http://hz.aibaodan.cn/gtgsyxwvuw.html

t = time.perf_counter()
来源：http://hz.ppjwa.cn/gtebadpaar.html

[U16] Py：命令行参数解析
来源：http://hz.ydjk.org.cn/gtndosqotc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.andypj.xyz/gtbvszetnt.html

[U17] Py：初始化日志
来源：http://hz.cheryme.top/gtnawyrgst.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhijiandao.cn/gtymgexguo.html

[U18] Py：预编译正则
来源：http://hz.sysykeji.top/gtasqonbuv.html

pat = re.compile(r"\d+")
来源：http://hz.sysykeji.top/gtdkbdqbnq.html

[U19] Py：正则替换带回调
来源：http://hz.kuanghao11.cn/gtygsscomg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xingfuxueyuan.xyz/gtpexrlbnq.html

[U20] Py：缓存函数结果
来源：http://hz.birdmap.top/gtimzyltuq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.fengsongda.top/gtpnytwkyf.html

[U21] Py：自定义上下文管理器
来源：http://hz.hnqzz.top/gtxvravthn.html

@contextlib.contextmanager
来源：http://hz.sxryk.cn/gtdounutnd.html

[U22] Py：矩阵转置
来源：http://hz.chenjidiqi.icu/gtayjrexze.html

list(zip(*m))
来源：http://hz.52xcode.cn/gtzfxivgrv.html

[U23] Py：分块读取大文件
来源：http://hz.xinyue.icu/gtueabskwd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.wangshuangyany.cn/gtfevpghvp.html

[U24] Py：路径操作
来源：http://hz.meibo888.top/gtbmkfudzm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangdashe.top/gtjcxfrxde.html

[U25] Py：CSV 按字典读
来源：http://hz.shzxlz.cn/gtcvwiwefy.html

csv.DictReader(f)
来源：http://hz.xinyue.icu/gtduignecb.html

[U26] Py：并发下载
来源：http://hz.daria6918.cn/gtlwyytwmx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sufxvd.cn/gtxkovginn.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtfamwvtib.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hnqzz.top/gtufrtbpdw.html

[U28] Py：类型别名
来源：http://hz.ywan-chungtsiang.top/gtffwywuza.html

UserId = int
来源：http://hz.gaohongyu789.top/gtnlwbrqam.html

[U29] Py：属性校验
来源：http://hz.zhijiandao.cn/gtcbygriyt.html

@property 与 @x.setter 配合
来源：http://hz.vqdsnc.cn/gtiivofxji.html

[U30] Py：数据类
来源：http://hz.nwbrower.top/gtkrpzogvu.html

@dataclass(slots=True)
来源：http://hz.ywan-chungtsiang.top/gtmdwyoayk.html

[U31] Py：单测
来源：http://hz.wangshuangyany.cn/gtaavemefz.html

python -m pytest -q
来源：http://hz.sweek.top/gtksukctpm.html

[U32] Py：代码格式化
来源：http://hz.hysaishi.cn/gtgudjmtuu.html

ruff format . && ruff check --fix .
来源：http://hz.sysykeji.top/gtyfetjkbs.html

[U33] Py：打包发布
来源：http://hz.gotoacloud.top/gtxcuogqhi.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ehwqpu.com/gtdmvlxwyn.html

[U34] Py：判断编码
来源：http://hz.jinghuilouyu.cn/gtwerkbome.html

chardet.detect(raw)
来源：http://hz.wangdashe.top/gtfrbuuuat.html

[U35] Py：发送邮件
来源：http://hz.wangdashe.top/gtjlauvdec.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.chenzaomai.com/gtefqllntl.html

[U36] Py：定时任务
来源：http://hz.yj20258888.top/gtiqzvkhmz.html

schedule.every(10).minutes.do(job)
来源：http://hz.ydjk.org.cn/gtwvxykdhy.html

[U37] Py：读写 Excel
来源：http://hz.yongpay.top/gtqlvnwmoz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xylfe.cn/gtdcwrmrff.html

[U38] Py：获取脚本所在目录
来源：http://hz.hfpthk.cn/gtaccrxxyu.html

Path(__file__).resolve().parent
来源：http://hz.chenzaomai.com/gtdgkevofk.html

[U39] Py：判断是否在交互环境
来源：http://hz.redwolf501.top/gtbuvyuvpz.html

sys.stdout.isatty()
来源：http://hz.shanyushiyangkeji.top/gtazprvdcc.html

[U40] Py：打印到标准错误
来源：http://hz.shzxlz.cn/gtkjdzzwxr.html

print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtbpxtlxlu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yongpay.top/gtvwqdqvre.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xuanzx.com/gtqdcnkffw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xziqi.cn/gtdahmnsjb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.aizwys.cn/gtrenjpcqm.html

[U43] PHP：声明命名空间
来源：http://hz.sufxvd.cn/gtafndrhyt.html

namespace App\Http;
来源：http://hz.jianghu66.top/gtuxnseqzh.html

[U44] PHP：开启严格类型
来源：http://hz.xuanzx.com/gtygrfkojt.html

declare(strict_types=1);
来源：http://hz.aibaodan.cn/gtmljalxhj.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhongyouzk.top/gtjhrcbzio.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtfujvegzo.html

[U46] PHP：可空类型
来源：http://hz.pycfn.com/gtdmrnspka.html

?string $name = null
来源：http://hz.birdmap.top/gtdbvwgugl.html

[U47] PHP：联合类型
来源：http://hz.ppjwa.cn/gtykgegfqx.html

int|string $id
来源：http://hz.xuetiantiany.cn/gthrxjojjk.html

[U48] PHP：纯枚举
来源：http://hz.tanke756.top/gtvkioqzff.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.guannengcc.top/gtissxvarn.html

[U49] PHP：只读属性
来源：http://hz.cdnleiting.top/gtilcklhry.html

public readonly string $name
来源：http://hz.zhaomingkeji.xyz/gtdwwjbtrh.html

[U50] PHP：构造器属性提升
来源：http://hz.haohaochexian.top/gtircwtnkh.html

public function __construct(private int $id) {}
来源：http://hz.zhoulong.xyz/gthlenxmti.html

[U51] PHP：数组解构
来源：http://hz.cucudq.cn/gtamxdsbgn.html

[$a, $b] = $arr;
来源：http://hz.ppjwa.cn/gtwfastnvm.html

[U52] PHP：箭头函数
来源：http://hz.yongpay.top/gtoplsvmgj.html

$double = fn($x) => $x * 2;
来源：http://hz.chenlongwang.top/gtwtelhsqt.html

[U53] PHP：空合并运算符
来源：http://hz.tanke756.top/gttgghcgbu.html

$v = $a ?? $b ?? "default";
来源：http://hz.fzhhl.top/gtytbyfbuf.html

[U54] PHP：空安全调用
来源：http://hz.jinqigfzy.top/gtseycjcbx.html

$obj?->method()
来源：http://hz.xuetiantiany.cn/gtpfjttajk.html

[U55] PHP：match 表达式
来源：http://hz.vqdsnc.cn/gtvwnulcxc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.iojbl.cn/gtxqlkzjse.html

[U56] PHP：命名参数
来源：http://hz.chenjidiqi.icu/gtnvqgcifk.html

f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gtbembgxok.html

[U57] PHP：字符串插值
来源：http://hz.yuanzhike.top/gtfutiqznw.html

"值: {$a}"
来源：http://hz.gzhubu.top/gtmmcgngyb.html

[U58] PHP：数组三件套
来源：http://hz.vqdsnc.cn/gtzozmdyfz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.pycfn.com/gttzgxjveg.html

[U59] PHP：自定义排序
来源：http://hz.zycfv.cn/gtdrlmncms.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yanxiufei.cn/gtmscuptmt.html

[U60] PHP：JSON 编解码
来源：http://hz.chenlongwang.top/gtokfqeqtk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.vqdsnc.cn/gtofexrpcw.html

[U61] PHP：正则
来源：http://hz.chenjidiqi.icu/gtewpeyqyg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gtbkzlxclx.html

[U62] PHP：日期对象
来源：http://hz.ywan-chungtsiang.top/gtfhokfquo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sxryk.cn/gtesfgvxpc.html

[U63] PHP：文件读写
来源：http://hz.chenjidiqi.icu/gtkcyqjlra.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhaomingkeji.xyz/gtoqzhcaxi.html

[U64] PHP：目录遍历
来源：http://hz.xuetiantiany.cn/gtmlvwqpxz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.chenlongwang.top/gtbfpbzdip.html

[U65] PHP：会话
来源：http://hz.shanyushiyangkeji.top/gtcvlgbkbo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.0kj1m.cn/gtvzhpflyu.html

[U66] PHP：设置 Cookie
来源：http://hz.daxiang520.top/gthbcarcxw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinqigfzy.top/gtmimfavcw.html

[U67] PHP：处理文件上传
来源：http://hz.gogol.net.cn/gtadpbqfxa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxinkj.top/gtmmqgxkoz.html

[U68] PHP：PDO 连接
来源：http://hz.daxiang520.top/gtbwqfueso.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.iojbl.cn/gtjodxsnuq.html

[U69] PHP：PDO 预处理
来源：http://hz.52xcode.cn/gtsxjsbzue.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.nanxinkj.top/gthnbxpagy.html

[U70] PHP：PDO 事务
来源：http://hz.feifeiyinyue.top/gtolcuqmdb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zdqjudy.top/gtkvflkqzh.html

[U71] PHP：抛出异常
来源：http://hz.cqqwz.cn/gtrqevetbd.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinqigfzy.top/gtejzwdzvf.html

[U72] PHP：写错误日志
来源：http://hz.meibo888.top/gtsnrvbebd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhiwuduotai.top/gttazkulal.html

[U73] PHP：读取 ini 配置
来源：http://hz.yueranfly.top/gtflmsaliq.html

parse_ini_file("config.ini", true)
来源：http://hz.9152youxi.cn/gtpqfrnnph.html

[U74] PHP：读取环境变量
来源：http://hz.dianchejie.cn/gtbdcmjrxw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yuanzhike.top/gtsuakxppc.html

[U75] PHP：依赖注入
来源：http://hz.pengpengdd.cyou/gtgbkhjvyi.html

composer require psr/container
来源：http://hz.cdnleiting.top/gtearciuvn.html

[U76] PHP：简单路由
来源：http://hz.chenjidiqi.icu/gtimklixvk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zdqjudy.top/gtmnzftdnr.html

[U77] PHP：模板渲染
来源：http://hz.nwbrower.top/gtxgatkfla.html

composer require twig/twig
来源：http://hz.fengsongda.top/gtjmgnfnlo.html

[U78] PHP：单元测试
来源：http://hz.chenjidiqi.icu/gtrfdkhyge.html

composer require --dev phpunit/phpunit
来源：http://hz.hnxiangtu.top/gthzdazlmi.html

[U79] PHP：静态分析
来源：http://hz.shzxlz.cn/gtboihhfhm.html

composer require --dev phpstan/phpstan
来源：http://hz.smart0.xyz/gtvvekrhey.html

[U80] PHP：代码规范修复
来源：http://hz.zdqjudy.top/gtbrzqeryu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ydjk.org.cn/gtfhthivrd.html

[U81] JS：初始化项目
来源：http://hz.kuanghao11.cn/gtemrayktk.html

npm init -y;  npm i express
来源：http://hz.tanke756.top/gtbqduyrqa.html

[U82] JS：package.json 脚本
来源：http://hz.shanyushiyangtech.top/gtnizjukes.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.tanke756.top/gtimmejjqh.html

[U83] JS：ES Module 导入导出
来源：http://hz.ydjk.org.cn/gtsadywjds.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.fzhhl.top/gtpzravmht.html

[U84] JS：CommonJS 写法
来源：http://hz.havefunace.top/gtbzthkzcl.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cheryme.top/gtqfbfodou.html

[U85] JS：可选链
来源：http://hz.xuanzx.com/gtforzazpv.html

a?.b?.c
来源：http://hz.zhongyouzk.top/gtbccjmnlu.html

[U86] JS：空值合并
来源：http://hz.fzhhl.top/gtxvrwbbaj.html

a ?? b
来源：http://hz.ydzc1.top/gtgfdsjcxp.html

[U87] JS：解构默认值
来源：http://hz.cashguo.top/gtndwbnonx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.fengsongda.top/gtebgndjfr.html

[U88] JS：对象展开合并
来源：http://hz.pengpengdd.cyou/gttbfykyfb.html

{ ...a, ...b }
来源：http://hz.yuxming.cn/gtlrtenxli.html

[U89] JS：数组去重
来源：http://hz.sysykeji.top/gtgairzqna.html

[...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtirgvovtc.html

[U90] JS：数字数组排序
来源：http://hz.bjfxy.top/gtosblxorl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtissmqnro.html

[U91] JS：对象键值遍历
来源：http://hz.shuidangran.top/gtiensthgm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cqqwz.cn/gtulipfhon.html

[U92] JS：深拷贝
来源：http://hz.kuanghao11.cn/gthbyaeakb.html

structuredClone(obj)
来源：http://hz.birdmap.top/gtzgvrbkbb.html

[U93] JS：模板字符串
来源：http://hz.shzxlz.cn/gtiekobrwj.html

`共 ${n} 条`
来源：http://hz.tanke756.top/gtipykhpve.html

[U94] JS：箭头函数
来源：http://hz.sufxvd.cn/gtsjdhjqyl.html

const double = x => x * 2;
来源：http://hz.svipenyu.cn/gtjyiinljj.html

[U95] JS：Promise 包装
来源：http://hz.nwbrower.top/gtsiqvitir.html

new Promise((resolve, reject) => {})
来源：http://hz.shuidangran.top/gtlulwtiki.html

[U96] JS：async/await 与异常
来源：http://hz.yj20258888.top/gtumvudbco.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtcovphuta.html

[U97] JS：并发请求
来源：http://hz.zhaomingkeji.xyz/gtmgmziclx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtzoztidts.html

[U98] JS：fetch 带 JSON
来源：http://hz.ppjwa.cn/gtwugodxon.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yuxming.cn/gtoslskikn.html

[U99] JS：事件监听
来源：http://hz.chenjidiqi.icu/gtcyvwicwj.html

el.addEventListener("click", e => {})
来源：http://hz.gotoacloud.top/gtihnpnzks.html

[U100] JS：DOM 查询
来源：http://hz.yvedp.cn/gtctwswxxf.html

document.querySelector(".item")
来源：http://hz.gaohongyu789.top/gtkiqelfyf.html

[U101] JS：classList 操作
来源：http://hz.gotoacloud.top/gtbvyzzbbr.html

el.classList.toggle("active")
来源：http://hz.gzhubu.top/gtjojshvyq.html

[U102] JS：本地存储
来源：http://hz.hfpthk.cn/gturqfcbuf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xingfuxueyuan.xyz/gtptzymwio.html

[U103] JS：定时器
来源：http://hz.nanxuanxn.top/gteohxybmz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhengqikj.top/gtaefkwfok.html

[U104] JS：防抖
来源：http://hz.hongshengwenyu.top/gtosfdzhtm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtuajhtdpg.html

[U105] JS：节流
来源：http://hz.quarkkingdee.top/gtuzokkzdh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.fzhhl.top/gthyuvjcar.html

[U106] JS：日期格式化
来源：http://hz.hnqzz.top/gtjnoprirs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yangfankeji.com/gtvzfmqzwj.html

[U107] JS：数字千分位
来源：http://hz.pengpengdd.cyou/gtcysolchy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hysaishi.cn/gtmlfmptgo.html

[U108] JS：随机整数
来源：http://hz.feifeiyinyue.top/gtytwigsdc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.mhx1999.top/gtzpnbthhe.html

[U109] JS：数组分组
来源：http://hz.sufxvd.cn/gteldgcxgp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xylfe.cn/gtpvcjzqmc.html

[U110] JS：数组分块
来源：http://hz.hongshengwenyu.top/gtoctrnmrq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenjidiqi.icu/gtnqzdxojd.html

[U111] JS：对象转 Map
来源：http://hz.zdqjudy.top/gtstoonxwo.html

new Map(Object.entries(obj))
来源：http://hz.tianlin.xyz/gtduuseyfc.html

[U112] JS：字符串补位
来源：http://hz.yangfankeji.com/gtgvekuqfv.html

"7".padStart(3, "0")
来源：http://hz.xylfe.cn/gtuyxsetyc.html

[U113] JS：正则替换全部
来源：http://hz.hywenlv.cn/gtbindblmd.html

s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtrmpuvdle.html

[U114] JS：JSON 深比较
来源：http://hz.zhiwuduotai.top/gtpihfyvst.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtnaydbnjo.html

[U115] JS：生成 UUID
来源：http://hz.0kj1m.cn/gtyfwpdbla.html

crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtfxjkmeqc.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shzxlz.cn/gtosjrbbmr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yvedp.cn/gtulwtgrxl.html

[U117] JS：单元测试
来源：http://hz.meibo888.top/gtlgafurhh.html

npm i -D vitest;  npx vitest
来源：http://hz.cdnleiting.top/gthmnllrxb.html

[U118] JS：开发服务器
来源：http://hz.zhoulong.xyz/gtaywfhzbb.html

npm i -D vite;  npx vite
来源：http://hz.gzhubu.top/gthyqomkno.html

[U119] JS：生产构建
来源：http://hz.chenjidiqi.icu/gtazpzdqxz.html

npx vite build
来源：http://hz.pycfn.com/gtdftstshf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.smart0.xyz/gtzznbyytf.html

import.meta.env.VITE_API_URL
来源：http://hz.zhiwuduotai.top/gthlmphbih.html

================================================================================
来源：http://hz.nanxinkj.top/gtgmmnyggc.html

统计汇总
来源：http://hz.xuetiantiany.cn/gtwncpxymk.html

================================================================================
来源：http://hz.yj202588.top/gtkoxxgdlw.html

按语言统计（条）：
来源：http://hz.haohaochexian.top/gtklzwukhc.html

Python ......... 252
来源：http://hz.daria6918.cn/gtakdmembu.html

PHP ............ 252
来源：http://hz.hfpthk.cn/gtuqnwoomu.html

JavaScript ..... 252
来源：http://hz.jiagoushi.top/gtfezwayeh.html

TypeScript ..... 212
来源：http://hz.chenjidiqi.icu/gtrkkxssst.html

Java ........... 212
来源：http://hz.aizwys.cn/gtcuvgvvyb.html

Go ............. 212
来源：http://hz.cashguo.top/gtnpwwyuri.html

Ruby ........... 212
来源：http://hz.kuanghao11.cn/gtqwjdfiks.html

C# ............. 212
来源：http://hz.zhoulong.xyz/gtdjnqltee.html

C .............. 30
来源：http://hz.yonumen.top/gtkcnzxqtp.html

C++ ............ 30
来源：http://hz.c1oappe.top/gtplsyioqm.html

SQL ............ 90
来源：http://hz.shanyushiyangkeji.top/gtbqkgzkap.html

Bash ........... 80
来源：http://hz.fzhhl.top/gtphirtqie.html

Kotlin ......... 15
来源：http://hz.daxiang520.top/gtzzgmauem.html

Swift .......... 15
来源：http://hz.meibo888.top/gtpyeoksbp.html

Lua ............ 10
来源：http://hz.smart0.xyz/gtsswwyosb.html

Perl ........... 10
来源：http://hz.chenjidiqi.icu/gtrdlvivsc.html

Scala .......... 10
来源：http://hz.xuetiantiany.cn/gtsxbjslnv.html

------------------------------------
来源：http://hz.sweek.top/gtulztzepm.html

合计 ........... 2106 条
来源：http://hz.haohaochexian.top/gtnhjvnjnk.html

按章节统计：
来源：http://hz.316326.xyz/gtasdhaauh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj20258.top/gtmuiqxmvm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.guannengcc.top/gtwetursdk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtlebhzgzd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.andypj.xyz/gtnhiyardi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.dianchejie.cn/gtxruxuuuq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtlaeepwkq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ydjk.org.cn/gtecmozswr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.316326.xyz/gtfxfihjfs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtrtuymotc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.svipenyu.cn/gtwgplezta.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gthrtfvwnw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gtcaxxkejb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtxswwxocg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jiagoushi.top/gtkhkwayta.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.redwolf501.top/gtgnkfxkms.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtvsbhxjxi.html

Q SQL 专题                              90
来源：http://hz.quarkkingdee.top/gtomtpvccr.html

R Bash 专题                             80
来源：http://hz.yj202588.top/gtpfxyldpi.html

S C / C++ 专题                          60
来源：http://hz.xziqi.cn/gtzmdhcain.html

T 其他语言补充                          60
来源：http://hz.yueranfly.top/gtybtlyvmm.html


<!-- 参考信息 -->