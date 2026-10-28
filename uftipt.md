代发 wailian999

[T49] Perl：函数
来源：http://hz.aizwys.cn/gtoqhjzbfa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jiagoushi.top/gtmrebpbro.html

[T50] Perl：逐行读文件
来源：http://hz.jiagoushi.top/gtgpzsmjea.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hywenlv.cn/gttchfrdzi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nwbrower.top/gtnjowaogi.html

[T51] Scala：Hello World
来源：http://hz.dashuyun.cn/gtwwuiifmg.html

println("Hello")
来源：http://hz.cucudq.cn/gthemuhpsv.html

[T52] Scala：变量
来源：http://hz.shanyushiyangkeji.top/gtpsmztsqb.html

val a = 1;  var b = 2
来源：http://hz.sweek.top/gtxiuutndg.html

[T53] Scala：字符串插值
来源：http://hz.shangyingyoupin.top/gtydednnjz.html

s"值: $b"
来源：http://hz.jlsjyb.cn/gtmlibpovx.html

[T54] Scala：集合映射
来源：http://hz.aibaodan.cn/gtcwnskfsh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yongpay.top/gttbpdkoiz.html

[T55] Scala：集合过滤
来源：http://hz.guannengcc.top/gtdficvjso.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shangyingyoupin.top/gtzrjrgotg.html

[T56] Scala：样例类
来源：http://hz.zhoulong.xyz/gtibjdsrsx.html

case class User(name: String, age: Int)
来源：http://hz.cheryme.top/gtrfpqgkyq.html

[T57] Scala：模式匹配
来源：http://hz.bjfxy.top/gtvkufkhxa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.smart0.xyz/gtoftfxmhx.html

[T58] Scala：函数定义
来源：http://hz.zdqjudy.top/gtdvzefmlr.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.redwolf501.top/gtxbkaznve.html

[T59] Scala：循环
来源：http://hz.shuidangran.top/gtrxbujcbm.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhaomingkeji.xyz/gtxflavmwb.html

[T60] Scala：折叠
来源：http://hz.xuanzx.com/gtutvsbjih.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ivvv.top/gttfbxflsl.html

================================================================================
来源：http://hz.cucudq.cn/gtopmxyofl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jiagoushi.top/gtszbrctat.html

================================================================================
来源：http://hz.iojbl.cn/gttxjlcqxp.html

[U01] Py：创建虚拟环境
来源：http://hz.tian-w.cn/gtnbksyzfq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhijiandao.cn/gtscpwwilv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yueranfly.top/gtdvbgfmdr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sweek.top/gtxbshyuvw.html

[U03] Py：加载 .env 配置
来源：http://hz.jinqigufen.top/gthtcclllm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yuanzhike.top/gtvaoguwhy.html

[U04] Py：变量调试打印
来源：http://hz.316326.xyz/gtdivxoczh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.chenlongwang.top/gtstyrkecv.html

[U05] Py：列表去重且保序
来源：http://hz.jinqigfzy.top/gtjdvhhlui.html

list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gtzqbkymyh.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtwjwyszje.html

{**a, **b}
来源：http://hz.yj20258.top/gtllgmdxyi.html

[U07] Py：反转字典键值
来源：http://hz.tanke756.top/gtokwuhrnc.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtwojruwfl.html

[U08] Py：展平二维列表
来源：http://hz.shangyingyoupin.top/gtiyoyvlnl.html

[y for x in nested for y in x]
来源：http://hz.gzhubu.top/gtnctiqiet.html

[U09] Py：字典取最大值的键
来源：http://hz.wangshuangyany.cn/gtsjrvnmxz.html

max(d, key=d.get)
来源：http://hz.chenjidiqi.icu/gtzjwpkdjf.html

[U10] Py：按值排序字典
来源：http://hz.hongshengwenyu.top/gtzrsotjog.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hfpthk.cn/gttuxdunro.html

[U11] Py：生成器表达式
来源：http://hz.chenjidiqi.icu/gtdytengbk.html

(x * 2 for x in arr)
来源：http://hz.nwbrower.top/gtsxizzmas.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.guowangkeji.top/gtbcxuuksb.html

Counter(arr).most_common(3)
来源：http://hz.vqdsnc.cn/gtcdsbatum.html

[U13] Py：固定长度队列
来源：http://hz.tian-w.cn/gtybcqbsrx.html

deque(maxlen=10)
来源：http://hz.hnxiangtu.top/gtqziyyhts.html

[U14] Py：分组收集到列表
来源：http://hz.nanxinkj.top/gtjcsocvcb.html

defaultdict(list)
来源：http://hz.cashguo.top/gtuzhbcdot.html

[U15] Py：高精度计时
来源：http://hz.aibaodan.cn/gtegdkyusy.html

t = time.perf_counter()
来源：http://hz.jyoumei.cn/gtgcallhwz.html

[U16] Py：命令行参数解析
来源：http://hz.xingfuxueyuan.xyz/gtihoiroas.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.smart0.xyz/gtjhcsejch.html

[U17] Py：初始化日志
来源：http://hz.yuxming.cn/gtjwfperxl.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.birdmap.top/gtjrckuypl.html

[U18] Py：预编译正则
来源：http://hz.hysaishi.cn/gtvikijlji.html

pat = re.compile(r"\d+")
来源：http://hz.yj20258.top/gtgqdnqsod.html

[U19] Py：正则替换带回调
来源：http://hz.9152youxi.cn/gtkvloujhz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxuanxn.top/gtaijhfckw.html

[U20] Py：缓存函数结果
来源：http://hz.yanxiufei.cn/gtuxbqunzv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yuanzhike.top/gthyyrsgox.html

[U21] Py：自定义上下文管理器
来源：http://hz.nanxuanxn.top/gtzqktjiky.html

@contextlib.contextmanager
来源：http://hz.quarkkingdee.top/gttemptoni.html

[U22] Py：矩阵转置
来源：http://hz.zycfv.cn/gtqqhjhibr.html

list(zip(*m))
来源：http://hz.xuetiantiany.cn/gtrxmfbptz.html

[U23] Py：分块读取大文件
来源：http://hz.jiagoushi.top/gtadkfparl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yangfankeji.com/gtlhqjjgaf.html

[U24] Py：路径操作
来源：http://hz.vqdsnc.cn/gtpggdobci.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ppjwa.cn/gtcccpatnb.html

[U25] Py：CSV 按字典读
来源：http://hz.svipenyu.cn/gtmksjxbgb.html

csv.DictReader(f)
来源：http://hz.xingfuxueyuan.xyz/gttmnmxmcp.html

[U26] Py：并发下载
来源：http://hz.tian-w.cn/gtnvqvqids.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.snrcjt.cn/gtzcxeodvd.html

[U27] Py：异步 HTTP
来源：http://hz.9152youxi.cn/gtcupqaxta.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yj202588.top/gtpwegnwzk.html

[U28] Py：类型别名
来源：http://hz.shanyushiyangtech.top/gtbptfhujr.html

UserId = int
来源：http://hz.ivvv.top/gteekkhijn.html

[U29] Py：属性校验
来源：http://hz.hfpthk.cn/gtjhmkrdru.html

@property 与 @x.setter 配合
来源：http://hz.mhx1999.top/gtwflwupor.html

[U30] Py：数据类
来源：http://hz.xuetiantiany.cn/gtkzzmrdgg.html

@dataclass(slots=True)
来源：http://hz.jlsjyb.cn/gtomkwxkza.html

[U31] Py：单测
来源：http://hz.yongpay.top/gtmujosljf.html

python -m pytest -q
来源：http://hz.wangshuangyany.cn/gtxaezqdna.html

[U32] Py：代码格式化
来源：http://hz.ydzc1.top/gtecozwung.html

ruff format . && ruff check --fix .
来源：http://hz.ywan-chungtsiang.top/gtlcotcxcv.html

[U33] Py：打包发布
来源：http://hz.zdqjudy.top/gtpwyveafb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shanyushiyangkeji.top/gtmcgxqfpf.html

[U34] Py：判断编码
来源：http://hz.quarkkingdee.top/gtlisvxjhh.html

chardet.detect(raw)
来源：http://hz.sxryk.cn/gtmjrpfrek.html

[U35] Py：发送邮件
来源：http://hz.hysaishi.cn/gtrldugicx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hysaishi.cn/gtjgbeydvj.html

[U36] Py：定时任务
来源：http://hz.xuetiantiany.cn/gtsaamapny.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhaomingkeji.xyz/gtavhokwzw.html

[U37] Py：读写 Excel
来源：http://hz.sysykeji.top/gtocxkzkzy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cdnleiting.top/gtrdkbgsey.html

[U38] Py：获取脚本所在目录
来源：http://hz.yueranfly.top/gtytjtbdia.html

Path(__file__).resolve().parent
来源：http://hz.yongpay.top/gtqxiampln.html

[U39] Py：判断是否在交互环境
来源：http://hz.cdnleiting.top/gtwhcgpqct.html

sys.stdout.isatty()
来源：http://hz.redwolf501.top/gtkphpgokc.html

[U40] Py：打印到标准错误
来源：http://hz.haohaochexian.top/gtqepufuta.html

print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gteynhzqnz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sysykeji.top/gtbshmfkor.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.fzhhl.top/gtlqlareuu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhoulong.xyz/gtcldaktez.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinyuanbaomall.cn/gtlfmmovcl.html

[U43] PHP：声明命名空间
来源：http://hz.cashguo.top/gtwmhutjza.html

namespace App\Http;
来源：http://hz.aizwys.cn/gtcxwpnvfa.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangtech.top/gtuwymmwen.html

declare(strict_types=1);
来源：http://hz.shanyushiyangtech.top/gtjahkbwih.html

[U45] PHP：类型声明与返回类型
来源：http://hz.smart0.xyz/gtjovgyhhe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.kuanghao11.cn/gtmfohxlvj.html

[U46] PHP：可空类型
来源：http://hz.yueranfly.top/gtgfqbnlxb.html

?string $name = null
来源：http://hz.gaohongyu789.top/gtpgmldlbu.html

[U47] PHP：联合类型
来源：http://hz.ybcxt.top/gttedkzaci.html

int|string $id
来源：http://hz.fengsongda.top/gtalnvjqcz.html

[U48] PHP：纯枚举
来源：http://hz.birdmap.top/gthruomasz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hywenlv.cn/gtwbxqqswx.html

[U49] PHP：只读属性
来源：http://hz.nanxuanxn.top/gtjxyxwuln.html

public readonly string $name
来源：http://hz.dianchejie.cn/gtwmnufpar.html

[U50] PHP：构造器属性提升
来源：http://hz.ehwqpu.com/gtvzdlifil.html

public function __construct(private int $id) {}
来源：http://hz.hywenlv.cn/gttfaznvss.html

[U51] PHP：数组解构
来源：http://hz.cqqwz.cn/gtamncqflj.html

[$a, $b] = $arr;
来源：http://hz.yangfankeji.com/gtoejdluik.html

[U52] PHP：箭头函数
来源：http://hz.hywenlv.cn/gtvylknwax.html

$double = fn($x) => $x * 2;
来源：http://hz.xinyue.icu/gtnuzsdyfz.html

[U53] PHP：空合并运算符
来源：http://hz.yongpay.top/gtlvjpkqsp.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinghuilouyu.cn/gtkzqvgjrf.html

[U54] PHP：空安全调用
来源：http://hz.ydzc1.top/gtmlpcnabb.html

$obj?->method()
来源：http://hz.yj20258.top/gtztmwwcms.html

[U55] PHP：match 表达式
来源：http://hz.jyoumei.cn/gtdhawpzos.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.redwolf501.top/gtxkwbhgef.html

[U56] PHP：命名参数
来源：http://hz.jyoumei.cn/gtjufbpdyh.html

f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtteelugqv.html

[U57] PHP：字符串插值
来源：http://hz.ydjk.org.cn/gtboglwbdh.html

"值: {$a}"
来源：http://hz.zhixingplan.top/gttsoeculs.html

[U58] PHP：数组三件套
来源：http://hz.daxiang520.top/gtcazrdosw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.wangdashe.top/gtpqlfvfyp.html

[U59] PHP：自定义排序
来源：http://hz.vqdsnc.cn/gtvokafahy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenzaomai.com/gthwevhaga.html

[U60] PHP：JSON 编解码
来源：http://hz.zhengqikj.top/gtnimxtoev.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tanke756.top/gtzqeonqmq.html

[U61] PHP：正则
来源：http://hz.feifeiyinyue.top/gtknjlelmd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gtwtngcfdw.html

[U62] PHP：日期对象
来源：http://hz.shuidangran.top/gtpqmatarv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yonumen.top/gtghsnrxgj.html

[U63] PHP：文件读写
来源：http://hz.ybcxt.top/gtslecivyh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xingfuxueyuan.xyz/gtiwwtzcux.html

[U64] PHP：目录遍历
来源：http://hz.ppjwa.cn/gtcjyfdzwp.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jinghuilouyu.cn/gtxahihqst.html

[U65] PHP：会话
来源：http://hz.yvedp.cn/gtdfeunydl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtrkirarew.html

[U66] PHP：设置 Cookie
来源：http://hz.cashguo.top/gtdgibuylp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.shzxlz.cn/gtbyjhjkag.html

[U67] PHP：处理文件上传
来源：http://hz.nanxinkj.top/gtyyozudpr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yvedp.cn/gtmctckhue.html

[U68] PHP：PDO 连接
来源：http://hz.meibo888.top/gtpxwjhosn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yueranfly.top/gthrvfxgwj.html

[U69] PHP：PDO 预处理
来源：http://hz.zhoulong.xyz/gtjdedbmkp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.andypj.xyz/gtndpqwtji.html

[U70] PHP：PDO 事务
来源：http://hz.pengpengdd.cyou/gtxrhwroug.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cdnleiting.top/gtdmbcswic.html

[U71] PHP：抛出异常
来源：http://hz.wangshuangyany.cn/gthuwdwxxu.html

throw new RuntimeException("失败", 500);
来源：http://hz.smart0.xyz/gtruitellr.html

[U72] PHP：写错误日志
来源：http://hz.hongshengwenyu.top/gttmyrpaxu.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ydzc1.top/gtdsyuyxnb.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhaomingkeji.xyz/gtdbivpfum.html

parse_ini_file("config.ini", true)
来源：http://hz.ehwqpu.com/gtydhdnsvy.html

[U74] PHP：读取环境变量
来源：http://hz.havefunace.top/gtgrzexeqe.html

getenv("APP_ENV") ?: "production"
来源：http://hz.52xcode.cn/gtoycaffpv.html

[U75] PHP：依赖注入
来源：http://hz.jinqigfzy.top/gtkzjspitj.html

composer require psr/container
来源：http://hz.yangfankeji.com/gtmwuudgcj.html

[U76] PHP：简单路由
来源：http://hz.nanxinkj.top/gtbutiorde.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yonumen.top/gtrzdwlogd.html

[U77] PHP：模板渲染
来源：http://hz.vqdsnc.cn/gthusgqwlx.html

composer require twig/twig
来源：http://hz.ywan-chungtsiang.top/gtuvwatbck.html

[U78] PHP：单元测试
来源：http://hz.yj20258888.top/gtjirxqfla.html

composer require --dev phpunit/phpunit
来源：http://hz.sxryk.cn/gtcrvudgpc.html

[U79] PHP：静态分析
来源：http://hz.zhongyouzk.top/gtwdrcrgvi.html

composer require --dev phpstan/phpstan
来源：http://hz.fzhhl.top/gtmmmvhabt.html

[U80] PHP：代码规范修复
来源：http://hz.shanyushiyangtech.top/gtwayonuaw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangshuangyany.cn/gtksaklhal.html

[U81] JS：初始化项目
来源：http://hz.zycfv.cn/gtcewulkhw.html

npm init -y;  npm i express
来源：http://hz.vqdsnc.cn/gtomxtgziq.html

[U82] JS：package.json 脚本
来源：http://hz.yueranfly.top/gtxjfhmgob.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yj20258.top/gtupkufxrb.html

[U83] JS：ES Module 导入导出
来源：http://hz.yuxming.cn/gtztxrtxet.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zdqjudy.top/gtuqqxnfur.html

[U84] JS：CommonJS 写法
来源：http://hz.jqgufenzy.top/gtxfjzwlwx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.fengsongda.top/gtzpfkyuks.html

[U85] JS：可选链
来源：http://hz.zhixingplan.top/gtfuthisvl.html

a?.b?.c
来源：http://hz.havefunace.top/gtfidnsubn.html

[U86] JS：空值合并
来源：http://hz.xuanzx.com/gteqrgerho.html

a ?? b
来源：http://hz.nanxuanxn.top/gtdfizavdr.html

[U87] JS：解构默认值
来源：http://hz.sysykeji.top/gtmecbnrfj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.svipenyu.cn/gtvrpywhus.html

[U88] JS：对象展开合并
来源：http://hz.yangfankeji.com/gtbbivsyjq.html

{ ...a, ...b }
来源：http://hz.fzhhl.top/gtninmjnre.html

[U89] JS：数组去重
来源：http://hz.nwbrower.top/gtdxxziwmi.html

[...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtopcrvfym.html

[U90] JS：数字数组排序
来源：http://hz.shangyingyoupin.top/gtgqulrqaj.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtmzcjuqho.html

[U91] JS：对象键值遍历
来源：http://hz.zhijiandao.cn/gtxggpadsz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.fengsongda.top/gtsfwhylhx.html

[U92] JS：深拷贝
来源：http://hz.svipenyu.cn/gtdrqstwkk.html

structuredClone(obj)
来源：http://hz.nwbrower.top/gtawwnqezr.html

[U93] JS：模板字符串
来源：http://hz.feifeiyinyue.top/gtwxwijsqv.html

`共 ${n} 条`
来源：http://hz.wangshuangyany.cn/gtfzaaqdot.html

[U94] JS：箭头函数
来源：http://hz.ppjwa.cn/gtjfdgmmnq.html

const double = x => x * 2;
来源：http://hz.tanke756.top/gtbaisezzc.html

[U95] JS：Promise 包装
来源：http://hz.smart0.xyz/gtaydsullu.html

new Promise((resolve, reject) => {})
来源：http://hz.ybcxt.top/gtqwthhzeo.html

[U96] JS：async/await 与异常
来源：http://hz.dashuyun.cn/gtzphirqjk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtbfbquapg.html

[U97] JS：并发请求
来源：http://hz.fzhhl.top/gtiptscpjx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtftmumdnp.html

[U98] JS：fetch 带 JSON
来源：http://hz.dashuyun.cn/gtvqwdrfai.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.vqdsnc.cn/gtoztelxvc.html

[U99] JS：事件监听
来源：http://hz.daria6918.cn/gtzxvyriud.html

el.addEventListener("click", e => {})
来源：http://hz.yvedp.cn/gtvpresnla.html

[U100] JS：DOM 查询
来源：http://hz.smart0.xyz/gtjzojvzoi.html

document.querySelector(".item")
来源：http://hz.tianlin.xyz/gtaiqargyz.html

[U101] JS：classList 操作
来源：http://hz.sysykeji.top/gteapnutfe.html

el.classList.toggle("active")
来源：http://hz.ywan-chungtsiang.top/gtzlgoonrf.html

[U102] JS：本地存储
来源：http://hz.cdnleiting.top/gtbmqbowcw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.haohaochexian.top/gtewtaawjv.html

[U103] JS：定时器
来源：http://hz.sweek.top/gtpinaxadf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.smart0.xyz/gttlavvmxo.html

[U104] JS：防抖
来源：http://hz.shanyushiyangtech.top/gttgyqliqm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtjezzydck.html

[U105] JS：节流
来源：http://hz.xziqi.cn/gtvjqbcqwk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.c1oappe.top/gtrpkdyobq.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gtjptjbgvb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhoulong.xyz/gtywhketrw.html

[U107] JS：数字千分位
来源：http://hz.bjfxy.top/gtjjlrbicx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jiagoushi.top/gtxphhcrhk.html

[U108] JS：随机整数
来源：http://hz.sysykeji.top/gtgpqfgagb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.svipenyu.cn/gtkaqqqyve.html

[U109] JS：数组分组
来源：http://hz.daria6918.cn/gtzpnkfdxg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtwyzjeeeo.html

[U110] JS：数组分块
来源：http://hz.xingfuxueyuan.xyz/gtfpyueqct.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.guowangkeji.top/gtdpzjfbds.html

[U111] JS：对象转 Map
来源：http://hz.ywan-chungtsiang.top/gtzfkueccw.html

new Map(Object.entries(obj))
来源：http://hz.xinyue.icu/gtivjjzyqm.html

[U112] JS：字符串补位
来源：http://hz.wangshuangyany.cn/gtdkkmvecy.html

"7".padStart(3, "0")
来源：http://hz.sweek.top/gtgxlkpcix.html

[U113] JS：正则替换全部
来源：http://hz.gotoacloud.top/gtkbvhgock.html

s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtawnvrccz.html

[U114] JS：JSON 深比较
来源：http://hz.9152youxi.cn/gtnecuwkpa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtdtppdoqu.html

[U115] JS：生成 UUID
来源：http://hz.gaohongyu789.top/gttdrbmuvy.html

crypto.randomUUID()
来源：http://hz.xinyue.icu/gttfqghdlg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhengqikj.top/gtdbwydsbb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hnqzz.top/gtvdvopjzb.html

[U117] JS：单元测试
来源：http://hz.jqgufenzy.top/gtfdgbekan.html

npm i -D vitest;  npx vitest
来源：http://hz.sysykeji.top/gtujzkpuyg.html

[U118] JS：开发服务器
来源：http://hz.tianlin.xyz/gtxajjheld.html

npm i -D vite;  npx vite
来源：http://hz.zhongyouzk.top/gtshxflnld.html

[U119] JS：生产构建
来源：http://hz.jyoumei.cn/gtmxudxtde.html

npx vite build
来源：http://hz.hnxiangtu.top/gtordghdxx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gotoacloud.top/gtdeoeauvm.html

import.meta.env.VITE_API_URL
来源：http://hz.ppjwa.cn/gtkednjxiu.html

================================================================================
来源：http://hz.aibaodan.cn/gtduembmfa.html

统计汇总
来源：http://hz.jinyuanbaomall.cn/gtyhwmdlcd.html

================================================================================
来源：http://hz.ydjk.org.cn/gtggpzztdz.html

按语言统计（条）：
来源：http://hz.jianghu66.top/gtcpoxqsoc.html

Python ......... 252
来源：http://hz.0kj1m.cn/gtklvskidr.html

PHP ............ 252
来源：http://hz.yj20258.top/gtripfunxv.html

JavaScript ..... 252
来源：http://hz.xziqi.cn/gtsngetzmm.html

TypeScript ..... 212
来源：http://hz.aizwys.cn/gtlvmzqaud.html

Java ........... 212
来源：http://hz.pycfn.com/gtfkebvbla.html

Go ............. 212
来源：http://hz.jlsjyb.cn/gtbanizaki.html

Ruby ........... 212
来源：http://hz.cqqwz.cn/gtimiujlks.html

C# ............. 212
来源：http://hz.ivvv.top/gtnpejaydn.html

C .............. 30
来源：http://hz.svipenyu.cn/gtyypnouxa.html

C++ ............ 30
来源：http://hz.jinyuanbaomall.cn/gtcmcqumfu.html

SQL ............ 90
来源：http://hz.kuanghao11.cn/gtjorbougi.html

Bash ........... 80
来源：http://hz.shanyushiyangkeji.top/gtsjcwzdvg.html

Kotlin ......... 15
来源：http://hz.c1oappe.top/gtmgqcggdh.html

Swift .......... 15
来源：http://hz.pycfn.com/gtlfjhdecs.html

Lua ............ 10
来源：http://hz.jinghuilouyu.cn/gtjaumzcqi.html

Perl ........... 10
来源：http://hz.shzxlz.cn/gtvzwmhfii.html

Scala .......... 10
来源：http://hz.ehwqpu.com/gterahgbzt.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtlekcwdcf.html

合计 ........... 2106 条
来源：http://hz.dianchejie.cn/gtdkwmhiac.html

按章节统计：
来源：http://hz.aibaodan.cn/gtjwjbrbcw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gtrwglqdsi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtulfwtsmu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtwmdhvohq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.havefunace.top/gtamdlowqk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ydjk.org.cn/gtcecrhipn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aibaodan.cn/gtevnzleos.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.wangdashe.top/gtudmyqhnv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zycfv.cn/gtspsxlgrr.html


<!-- 参考信息 -->