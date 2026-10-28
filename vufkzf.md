代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://hz.tanke756.top/gtlufkycbc.html

[T51] Scala：Hello World
来源：http://hz.yvedp.cn/gtthwwgrdq.html

println("Hello")
来源：http://hz.yangfankeji.com/gtorwtdygl.html

[T52] Scala：变量
来源：http://hz.yonumen.top/gtnnzxgelw.html

val a = 1;  var b = 2
来源：http://hz.dashuyun.cn/gtrijwiene.html

[T53] Scala：字符串插值
来源：http://hz.hfpthk.cn/gtcrvlgfit.html

s"值: $b"
来源：http://hz.quarkkingdee.top/gtmcocmxcw.html

[T54] Scala：集合映射
来源：http://hz.hnqzz.top/gtsmtnjprf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtfgwoxzks.html

[T55] Scala：集合过滤
来源：http://hz.shangyingyoupin.top/gtivikwklv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shangyingyoupin.top/gtyswqndlp.html

[T56] Scala：样例类
来源：http://hz.wangdashe.top/gthdtwgvww.html

case class User(name: String, age: Int)
来源：http://hz.xuetiantiany.cn/gtcokferce.html

[T57] Scala：模式匹配
来源：http://hz.jianghu66.top/gtbalnsdhr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhongyouzk.top/gtyvuojtvc.html

[T58] Scala：函数定义
来源：http://hz.svipenyu.cn/gtvovfaqmv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shuidangran.top/gtucwymzjq.html

[T59] Scala：循环
来源：http://hz.hnxiangtu.top/gtvvextvsg.html

for (i <- 1 to 10) println(i)
来源：http://hz.dashuyun.cn/gtrrkszszb.html

[T60] Scala：折叠
来源：http://hz.jqgufenzy.top/gtrmbvhawx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cashguo.top/gtjszjazmo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrdewpqlt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tianlin.xyz/gttiefkcay.html

================================================================================
来源：http://hz.cucudq.cn/gtqvfkiypi.html

[U01] Py：创建虚拟环境
来源：http://hz.ybcxt.top/gtqifkhyyv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hnqzz.top/gtsmeyjkvr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.dashuyun.cn/gtvrzzfjhd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenzaomai.com/gtqabpfimx.html

[U03] Py：加载 .env 配置
来源：http://hz.316326.xyz/gtqtkwdbma.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hfpthk.cn/gtwulmnyxc.html

[U04] Py：变量调试打印
来源：http://hz.dashuyun.cn/gtejztitpn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yueranfly.top/gtcaawwnxh.html

[U05] Py：列表去重且保序
来源：http://hz.xziqi.cn/gtoqzfuyaa.html

list(dict.fromkeys(arr))
来源：http://hz.yvedp.cn/gtclitrttc.html

[U06] Py：合并两个字典
来源：http://hz.yvedp.cn/gtivnjahsm.html

{**a, **b}
来源：http://hz.shangyingyoupin.top/gtbvcbvxwi.html

[U07] Py：反转字典键值
来源：http://hz.yj20258.top/gtasecgodd.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtzxccqlfr.html

[U08] Py：展平二维列表
来源：http://hz.wangdashe.top/gtatluzxbu.html

[y for x in nested for y in x]
来源：http://hz.xziqi.cn/gtznwarfkr.html

[U09] Py：字典取最大值的键
来源：http://hz.ehwqpu.com/gtrohqbiff.html

max(d, key=d.get)
来源：http://hz.quarkkingdee.top/gtkveejust.html

[U10] Py：按值排序字典
来源：http://hz.0kj1m.cn/gtmpivdduu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ivvv.top/gtermhzbvd.html

[U11] Py：生成器表达式
来源：http://hz.chenlongwang.top/gtddqdfrul.html

(x * 2 for x in arr)
来源：http://hz.dashuyun.cn/gtvtaqlwqa.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cdnleiting.top/gttazrrjox.html

Counter(arr).most_common(3)
来源：http://hz.ppjwa.cn/gtwiiahtra.html

[U13] Py：固定长度队列
来源：http://hz.kuanghao11.cn/gtphphrexf.html

deque(maxlen=10)
来源：http://hz.mhx1999.top/gtxdwtamph.html

[U14] Py：分组收集到列表
来源：http://hz.fzhhl.top/gtqwxzvtdv.html

defaultdict(list)
来源：http://hz.wangshuangyany.cn/gtaxusjiiv.html

[U15] Py：高精度计时
来源：http://hz.xuanzx.com/gtslzpixdc.html

t = time.perf_counter()
来源：http://hz.ywan-chungtsiang.top/gtepkgxyfs.html

[U16] Py：命令行参数解析
来源：http://hz.jyoumei.cn/gtrhhppkpi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ehwqpu.com/gtocirvevz.html

[U17] Py：初始化日志
来源：http://hz.tanke756.top/gteftpqgmj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fengsongda.top/gtdygahuaf.html

[U18] Py：预编译正则
来源：http://hz.wangshuangyany.cn/gtddbxaiqh.html

pat = re.compile(r"\d+")
来源：http://hz.pengpengdd.cyou/gtwuuftrva.html

[U19] Py：正则替换带回调
来源：http://hz.fzhhl.top/gthomsipdd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj202588.top/gtgxsifvmy.html

[U20] Py：缓存函数结果
来源：http://hz.ppjwa.cn/gtzllcivtm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yanxiufei.cn/gtpvvemkfe.html

[U21] Py：自定义上下文管理器
来源：http://hz.gzhubu.top/gtrlvuynul.html

@contextlib.contextmanager
来源：http://hz.meibo888.top/gtubzlukil.html

[U22] Py：矩阵转置
来源：http://hz.gotoacloud.top/gtmsvrqazt.html

list(zip(*m))
来源：http://hz.shanyushiyangkeji.top/gtbuaplfak.html

[U23] Py：分块读取大文件
来源：http://hz.sxryk.cn/gtyxzbglbg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.aizwys.cn/gtmksmftnc.html

[U24] Py：路径操作
来源：http://hz.9152youxi.cn/gtqstuhetm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jiagoushi.top/gtlqjvbvgm.html

[U25] Py：CSV 按字典读
来源：http://hz.zhaomingkeji.xyz/gtoitmhdyj.html

csv.DictReader(f)
来源：http://hz.ivvv.top/gtqpvdgvpz.html

[U26] Py：并发下载
来源：http://hz.chenlongwang.top/gtygkfktwa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.smart0.xyz/gtqfeyoslq.html

[U27] Py：异步 HTTP
来源：http://hz.ybcxt.top/gtwavptisj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sxryk.cn/gtffcdsonn.html

[U28] Py：类型别名
来源：http://hz.jqgfzy.top/gtjpyqyfek.html

UserId = int
来源：http://hz.chenlongwang.top/gtuafgshns.html

[U29] Py：属性校验
来源：http://hz.daria6918.cn/gtntkxyakj.html

@property 与 @x.setter 配合
来源：http://hz.yonumen.top/gtiyvocikg.html

[U30] Py：数据类
来源：http://hz.xuetiantiany.cn/gtnijqmntm.html

@dataclass(slots=True)
来源：http://hz.52xcode.cn/gtulmrbemv.html

[U31] Py：单测
来源：http://hz.andypj.xyz/gtktnumasf.html

python -m pytest -q
来源：http://hz.hnxiangtu.top/gthrggfvoj.html

[U32] Py：代码格式化
来源：http://hz.xinyue.icu/gtyfylugpi.html

ruff format . && ruff check --fix .
来源：http://hz.daria6918.cn/gtidcfabmq.html

[U33] Py：打包发布
来源：http://hz.fzhhl.top/gtcolublzb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.dianchejie.cn/gtxraitcwl.html

[U34] Py：判断编码
来源：http://hz.fzhhl.top/gtescdecjt.html

chardet.detect(raw)
来源：http://hz.wangdashe.top/gtubeaqybw.html

[U35] Py：发送邮件
来源：http://hz.yj202588.top/gthdemmjyk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zycfv.cn/gtglafddjl.html

[U36] Py：定时任务
来源：http://hz.bjfxy.top/gthupegaar.html

schedule.every(10).minutes.do(job)
来源：http://hz.ydzc1.top/gtljwqkbsl.html

[U37] Py：读写 Excel
来源：http://hz.zdqjudy.top/gtnzshlemc.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jiagoushi.top/gtghjqlouu.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhongyouzk.top/gtlzycypcc.html

Path(__file__).resolve().parent
来源：http://hz.tianlin.xyz/gtwlrgkzov.html

[U39] Py：判断是否在交互环境
来源：http://hz.sxryk.cn/gtogyggtin.html

sys.stdout.isatty()
来源：http://hz.zhongyouzk.top/gtqkcqucik.html

[U40] Py：打印到标准错误
来源：http://hz.zhongyouzk.top/gtkremmcnw.html

print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtxhdcxcqz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yuanzhike.top/gtragtuler.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.andypj.xyz/gtvakjdksn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.dianchejie.cn/gtkykeumeu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.guowangkeji.top/gtixebkjgw.html

[U43] PHP：声明命名空间
来源：http://hz.ywan-chungtsiang.top/gtaqqfpbcd.html

namespace App\Http;
来源：http://hz.snrcjt.cn/gthavhvhbk.html

[U44] PHP：开启严格类型
来源：http://hz.zhaomingkeji.xyz/gtjtqzxrqi.html

declare(strict_types=1);
来源：http://hz.chenjidiqi.icu/gthovnsnss.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ywan-chungtsiang.top/gtvndtkkrf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtcwjoploj.html

[U46] PHP：可空类型
来源：http://hz.haohaochexian.top/gtlylkqhac.html

?string $name = null
来源：http://hz.cashguo.top/gtnyisboee.html

[U47] PHP：联合类型
来源：http://hz.smart0.xyz/gtpvixjlur.html

int|string $id
来源：http://hz.yj202588.top/gtjgepfyqd.html

[U48] PHP：纯枚举
来源：http://hz.zhaomingkeji.xyz/gtqcalhsjj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.chenlongwang.top/gtjkwlmxdh.html

[U49] PHP：只读属性
来源：http://hz.iojbl.cn/gtfdzgkbmb.html

public readonly string $name
来源：http://hz.ydzc1.top/gtjnfruodf.html

[U50] PHP：构造器属性提升
来源：http://hz.jianghu66.top/gtbmqgbars.html

public function __construct(private int $id) {}
来源：http://hz.hongshengwenyu.top/gtslazdvgy.html

[U51] PHP：数组解构
来源：http://hz.andypj.xyz/gtkaucizvv.html

[$a, $b] = $arr;
来源：http://hz.iojbl.cn/gtmzlsieqe.html

[U52] PHP：箭头函数
来源：http://hz.nanxuanxn.top/gtkilfloga.html

$double = fn($x) => $x * 2;
来源：http://hz.mhx1999.top/gtmfqocaii.html

[U53] PHP：空合并运算符
来源：http://hz.fzhhl.top/gtkkwkpwjy.html

$v = $a ?? $b ?? "default";
来源：http://hz.sxryk.cn/gtkmpbzoey.html

[U54] PHP：空安全调用
来源：http://hz.c1oappe.top/gtxwnntnog.html

$obj?->method()
来源：http://hz.yonumen.top/gtdvvhpdow.html

[U55] PHP：match 表达式
来源：http://hz.shanyushiyangkeji.top/gtyaqpuvba.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gogol.net.cn/gthlgesqto.html

[U56] PHP：命名参数
来源：http://hz.ivvv.top/gtvngykcmq.html

f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtohwqrlmc.html

[U57] PHP：字符串插值
来源：http://hz.sysykeji.top/gtyqrzzmke.html

"值: {$a}"
来源：http://hz.daxiang520.top/gtvutdgwov.html

[U58] PHP：数组三件套
来源：http://hz.c1oappe.top/gtyolcxcls.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gotoacloud.top/gtfwkekyok.html

[U59] PHP：自定义排序
来源：http://hz.kuanghao11.cn/gtpnyjpbda.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gtrpdbpwiw.html

[U60] PHP：JSON 编解码
来源：http://hz.zhaomingkeji.xyz/gtnbicidhq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgufenzy.top/gtzyplpjpe.html

[U61] PHP：正则
来源：http://hz.xylfe.cn/gtiwyfmofe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sxryk.cn/gttlmkaomo.html

[U62] PHP：日期对象
来源：http://hz.jlsjyb.cn/gtjrpcqkeu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhiwuduotai.top/gtfungvbhq.html

[U63] PHP：文件读写
来源：http://hz.sysykeji.top/gtpmdhxjvz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xylfe.cn/gtuahysnjt.html

[U64] PHP：目录遍历
来源：http://hz.snrcjt.cn/gtposhsety.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.aibaodan.cn/gtvzyqojyr.html

[U65] PHP：会话
来源：http://hz.haohaochexian.top/gtrguvcoqb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hongshengwenyu.top/gtbkfgqrot.html

[U66] PHP：设置 Cookie
来源：http://hz.tianlin.xyz/gtcycwioao.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hywenlv.cn/gtjnzcsokx.html

[U67] PHP：处理文件上传
来源：http://hz.zhijiandao.cn/gtrfvdwxnc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yonumen.top/gtfpqqhils.html

[U68] PHP：PDO 连接
来源：http://hz.shanyushiyangkeji.top/gtmonchcuh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.nwbrower.top/gtvcbtssbz.html

[U69] PHP：PDO 预处理
来源：http://hz.jiagoushi.top/gtijoebnkg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sufxvd.cn/gtpgncpvhp.html

[U70] PHP：PDO 事务
来源：http://hz.iojbl.cn/gtuntgrayy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shangyingyoupin.top/gtpljaaclf.html

[U71] PHP：抛出异常
来源：http://hz.yueranfly.top/gtkpycqimf.html

throw new RuntimeException("失败", 500);
来源：http://hz.yonumen.top/gtzmisporu.html

[U72] PHP：写错误日志
来源：http://hz.ivvv.top/gtprocixsw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.bjfxy.top/gtpninbwfl.html

[U73] PHP：读取 ini 配置
来源：http://hz.vqdsnc.cn/gtqrouhzod.html

parse_ini_file("config.ini", true)
来源：http://hz.0kj1m.cn/gtkcloxkzt.html

[U74] PHP：读取环境变量
来源：http://hz.daria6918.cn/gtlpddfvny.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yongpay.top/gtjeianhep.html

[U75] PHP：依赖注入
来源：http://hz.xingfuxueyuan.xyz/gtpxzmdpla.html

composer require psr/container
来源：http://hz.feifeiyinyue.top/gtijcerdfa.html

[U76] PHP：简单路由
来源：http://hz.tianlin.xyz/gtsdghbmbc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jinghuilouyu.cn/gtmijapess.html

[U77] PHP：模板渲染
来源：http://hz.zhijiandao.cn/gtqmuxzfxb.html

composer require twig/twig
来源：http://hz.xingfuxueyuan.xyz/gtairzckrn.html

[U78] PHP：单元测试
来源：http://hz.zhijiandao.cn/gtpyfvrcry.html

composer require --dev phpunit/phpunit
来源：http://hz.zdqjudy.top/gtmcnlczoz.html

[U79] PHP：静态分析
来源：http://hz.ehwqpu.com/gtitohwmzd.html

composer require --dev phpstan/phpstan
来源：http://hz.sweek.top/gtgmzysflg.html

[U80] PHP：代码规范修复
来源：http://hz.wangshuangyany.cn/gtywjefkxz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hongshengwenyu.top/gtlrswukrf.html

[U81] JS：初始化项目
来源：http://hz.zhoulong.xyz/gtgmrwplvg.html

npm init -y;  npm i express
来源：http://hz.jinghuilouyu.cn/gtcmwxreyo.html

[U82] JS：package.json 脚本
来源：http://hz.guannengcc.top/gtcghjkevb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.0kj1m.cn/gtvdrkioac.html

[U83] JS：ES Module 导入导出
来源：http://hz.shuidangran.top/gtofwbxqng.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zycfv.cn/gtzcpzwmav.html

[U84] JS：CommonJS 写法
来源：http://hz.hfpthk.cn/gtsnooicas.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yj20258888.top/gtsmbiloxq.html

[U85] JS：可选链
来源：http://hz.jinyuanbaomall.cn/gtrdqsfhdo.html

a?.b?.c
来源：http://hz.dianchejie.cn/gtlfsvhqro.html

[U86] JS：空值合并
来源：http://hz.yongpay.top/gthfnjoxmt.html

a ?? b
来源：http://hz.jinqigfzy.top/gtetlivqnh.html

[U87] JS：解构默认值
来源：http://hz.hfpthk.cn/gthnuzlnwz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.nanxinkj.top/gtikxnlxer.html

[U88] JS：对象展开合并
来源：http://hz.sweek.top/gtftlqtove.html

{ ...a, ...b }
来源：http://hz.yuxming.cn/gtfoxyswhx.html

[U89] JS：数组去重
来源：http://hz.jlsjyb.cn/gtisrkanas.html

[...new Set(arr)]
来源：http://hz.chenzaomai.com/gtzpcxtzgw.html

[U90] JS：数字数组排序
来源：http://hz.chenlongwang.top/gtfcyhxxfn.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtjlakziuj.html

[U91] JS：对象键值遍历
来源：http://hz.shangyingyoupin.top/gtodavwzcu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.tanke756.top/gtpspciyqz.html

[U92] JS：深拷贝
来源：http://hz.xinyue.icu/gtdzzqmasl.html

structuredClone(obj)
来源：http://hz.gotoacloud.top/gtaobewicf.html

[U93] JS：模板字符串
来源：http://hz.xylfe.cn/gthipkkspv.html

`共 ${n} 条`
来源：http://hz.gogol.net.cn/gtehwpzuac.html

[U94] JS：箭头函数
来源：http://hz.jlsjyb.cn/gtvenemske.html

const double = x => x * 2;
来源：http://hz.birdmap.top/gtwokkefzs.html

[U95] JS：Promise 包装
来源：http://hz.shangyingyoupin.top/gtuzmspabi.html

new Promise((resolve, reject) => {})
来源：http://hz.mhx1999.top/gtravhvvam.html

[U96] JS：async/await 与异常
来源：http://hz.cheryme.top/gtpixntotn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cucudq.cn/gtvgptkkuk.html

[U97] JS：并发请求
来源：http://hz.yj20258888.top/gtqgmmokmy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtjnfjaxgb.html

[U98] JS：fetch 带 JSON
来源：http://hz.ivvv.top/gtehsjykpt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xylfe.cn/gtuconqczx.html

[U99] JS：事件监听
来源：http://hz.jyoumei.cn/gtevjltkkp.html

el.addEventListener("click", e => {})
来源：http://hz.yj202588.top/gtqetspjww.html

[U100] JS：DOM 查询
来源：http://hz.ivvv.top/gtvigzqxfj.html

document.querySelector(".item")
来源：http://hz.andypj.xyz/gtmsqznobr.html

[U101] JS：classList 操作
来源：http://hz.xziqi.cn/gtgzrfpcpq.html

el.classList.toggle("active")
来源：http://hz.zhaomingkeji.xyz/gtlvuajxlt.html

[U102] JS：本地存储
来源：http://hz.xinyue.icu/gtgbraflzm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yj20258.top/gtrufvxsmk.html

[U103] JS：定时器
来源：http://hz.shanyushiyangkeji.top/gtbzjgdyhw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cheryme.top/gtxrvvzhem.html

[U104] JS：防抖
来源：http://hz.jlsjyb.cn/gtiqxafjum.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtewsnozcn.html

[U105] JS：节流
来源：http://hz.jyoumei.cn/gthzjltmof.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.nanxuanxn.top/gtwioahenx.html

[U106] JS：日期格式化
来源：http://hz.shangyingyoupin.top/gtslrywkzp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.aibaodan.cn/gtntpctflb.html

[U107] JS：数字千分位
来源：http://hz.zdqjudy.top/gtopuvszqw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.guowangkeji.top/gtwwgnuoxz.html

[U108] JS：随机整数
来源：http://hz.sxryk.cn/gtpxxpaqsv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xuetiantiany.cn/gtserqnrxy.html

[U109] JS：数组分组
来源：http://hz.gotoacloud.top/gtfzprgzfi.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtlwdvaspz.html

[U110] JS：数组分块
来源：http://hz.smart0.xyz/gtpohnzgfj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.daxiang520.top/gtjhzstale.html

[U111] JS：对象转 Map
来源：http://hz.cucudq.cn/gtisjxdbof.html

new Map(Object.entries(obj))
来源：http://hz.ivvv.top/gttopctrxp.html

[U112] JS：字符串补位
来源：http://hz.0kj1m.cn/gtubibekub.html

"7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtmjxmjwmy.html

[U113] JS：正则替换全部
来源：http://hz.wangdashe.top/gtmvatrkwe.html

s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtwnftuxda.html

[U114] JS：JSON 深比较
来源：http://hz.sxryk.cn/gtxqyokroo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.birdmap.top/gtprgpqnjo.html

[U115] JS：生成 UUID
来源：http://hz.tanke756.top/gtvykcbckn.html

crypto.randomUUID()
来源：http://hz.316326.xyz/gtkrkqgnkn.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shuidangran.top/gtugrxvbio.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jyoumei.cn/gtqaelwjpy.html

[U117] JS：单元测试
来源：http://hz.tanke756.top/gtdkzlwgid.html

npm i -D vitest;  npx vitest
来源：http://hz.wangshuangyany.cn/gtsixazpdy.html

[U118] JS：开发服务器
来源：http://hz.sysykeji.top/gtwdnychyh.html

npm i -D vite;  npx vite
来源：http://hz.nanxinkj.top/gtbbolhxep.html

[U119] JS：生产构建
来源：http://hz.gotoacloud.top/gttxrurily.html

npx vite build
来源：http://hz.feifeiyinyue.top/gtjosnadkb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.guowangkeji.top/gticuttauj.html

import.meta.env.VITE_API_URL
来源：http://hz.meibo888.top/gtyapotcym.html

================================================================================
来源：http://hz.fengsongda.top/gtikxaypta.html

统计汇总
来源：http://hz.yj20258.top/gtbmikvsnx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtcfriagva.html

按语言统计（条）：
来源：http://hz.hammf.cn/gtphudmmlo.html

Python ......... 252
来源：http://hz.hywenlv.cn/gtozayjiar.html

PHP ............ 252
来源：http://hz.xingfuxueyuan.xyz/gtuvcqqnhh.html

JavaScript ..... 252
来源：http://hz.jlsjyb.cn/gtgcjarynm.html

TypeScript ..... 212
来源：http://hz.tianlin.xyz/gttegtfljm.html

Java ........... 212
来源：http://hz.guannengcc.top/gtslbgbmwu.html

Go ............. 212
来源：http://hz.yj202588.top/gtpzgkbzrj.html

Ruby ........... 212
来源：http://hz.pengpengdd.cyou/gtvacgcrdg.html

C# ............. 212
来源：http://hz.wangshuangyany.cn/gtzlwnmmhh.html

C .............. 30
来源：http://hz.kuanghao11.cn/gtvizwxlkm.html

C++ ............ 30
来源：http://hz.gaohongyu789.top/gtrjazdlom.html

SQL ............ 90
来源：http://hz.svipenyu.cn/gtcrscuxtn.html

Bash ........... 80
来源：http://hz.haohaochexian.top/gtrquimmfk.html

Kotlin ......... 15
来源：http://hz.xziqi.cn/gtvzueifxs.html

Swift .......... 15
来源：http://hz.daria6918.cn/gtfxlwzwuv.html

Lua ............ 10
来源：http://hz.zycfv.cn/gtqatsypoy.html

Perl ........... 10
来源：http://hz.yj20258.top/gtrtjlzooe.html

Scala .......... 10
来源：http://hz.zhongyouzk.top/gtujqhscmc.html

------------------------------------
来源：http://hz.yvedp.cn/gtkrixlzfj.html

合计 ........... 2106 条
来源：http://hz.jinyuanbaomall.cn/gtopryourb.html

按章节统计：
来源：http://hz.cashguo.top/gtgzyrlbzj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.pycfn.com/gteyzdecop.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xingfuxueyuan.xyz/gteqmkyhdl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtzkhhvciv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xuetiantiany.cn/gtoccvugqw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.andypj.xyz/gtiqtyxwvs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.quarkkingdee.top/gttpkvfqci.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtijsetpew.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gtgsgxsohm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtklimahic.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gthxgpguov.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtodsadnia.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtdkijzfml.html


<!-- 参考信息 -->