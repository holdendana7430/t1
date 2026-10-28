代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.pycfn.com/gtfuaoimog.html

[T55] Scala：集合过滤
来源：http://hz.fengsongda.top/gtydfxvvke.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydzc1.top/gtzmodgtbl.html

[T56] Scala：样例类
来源：http://hz.9152youxi.cn/gtpfcpgpaz.html

case class User(name: String, age: Int)
来源：http://hz.yvedp.cn/gtimzgvowg.html

[T57] Scala：模式匹配
来源：http://hz.svipenyu.cn/gtspryaizk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sufxvd.cn/gtqjuapcof.html

[T58] Scala：函数定义
来源：http://hz.xylfe.cn/gtzhnojezf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj202588.top/gtgzsqsmrv.html

[T59] Scala：循环
来源：http://hz.hywenlv.cn/gtxpwjbrpp.html

for (i <- 1 to 10) println(i)
来源：http://hz.pengpengdd.cyou/gtrqptqxou.html

[T60] Scala：折叠
来源：http://hz.hysaishi.cn/gtxdzqlfan.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hfpthk.cn/gtztzmddsw.html

================================================================================
来源：http://hz.tanke756.top/gtiypuswtt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxuanxn.top/gtiosuhrml.html

================================================================================
来源：http://hz.yangfankeji.com/gtzcvnqema.html

[U01] Py：创建虚拟环境
来源：http://hz.vqdsnc.cn/gtqhemntwd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daxiang520.top/gtuxuihutx.html

[U02] Py：导出 / 安装依赖
来源：http://hz.guowangkeji.top/gtqcjbfywl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.quarkkingdee.top/gtxoowdfnt.html

[U03] Py：加载 .env 配置
来源：http://hz.tian-w.cn/gtwovckkdy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zycfv.cn/gtwblcqdbo.html

[U04] Py：变量调试打印
来源：http://hz.xingfuxueyuan.xyz/gtgyivckfq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yanxiufei.cn/gtycevsfkc.html

[U05] Py：列表去重且保序
来源：http://hz.bjfxy.top/gtzysexifr.html

list(dict.fromkeys(arr))
来源：http://hz.52xcode.cn/gtqcnmojys.html

[U06] Py：合并两个字典
来源：http://hz.nwbrower.top/gtbxdbyvgy.html

{**a, **b}
来源：http://hz.shangyingyoupin.top/gtirybdikb.html

[U07] Py：反转字典键值
来源：http://hz.hywenlv.cn/gtrtwhbxcr.html

{v: k for k, v in d.items()}
来源：http://hz.daria6918.cn/gtiwtjjbhg.html

[U08] Py：展平二维列表
来源：http://hz.jqgfzy.top/gtqzphrtyd.html

[y for x in nested for y in x]
来源：http://hz.sweek.top/gtspblwqqt.html

[U09] Py：字典取最大值的键
来源：http://hz.chenjidiqi.icu/gtigqlxvqb.html

max(d, key=d.get)
来源：http://hz.quarkkingdee.top/gtcfgqnxnr.html

[U10] Py：按值排序字典
来源：http://hz.ydjk.org.cn/gtmlpadwzj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.daria6918.cn/gtsaxulkko.html

[U11] Py：生成器表达式
来源：http://hz.haohaochexian.top/gtcvpvvrue.html

(x * 2 for x in arr)
来源：http://hz.iojbl.cn/gtrmvefdza.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.havefunace.top/gtskcqcqxi.html

Counter(arr).most_common(3)
来源：http://hz.xuetiantiany.cn/gtlnwdqwfp.html

[U13] Py：固定长度队列
来源：http://hz.xuetiantiany.cn/gthqjikawo.html

deque(maxlen=10)
来源：http://hz.shangyingyoupin.top/gtpnyzunpu.html

[U14] Py：分组收集到列表
来源：http://hz.zycfv.cn/gtwzwlvjvm.html

defaultdict(list)
来源：http://hz.dashuyun.cn/gtvlxegpno.html

[U15] Py：高精度计时
来源：http://hz.xuetiantiany.cn/gtjzxoqapm.html

t = time.perf_counter()
来源：http://hz.smart0.xyz/gthhhjmqlo.html

[U16] Py：命令行参数解析
来源：http://hz.zhijiandao.cn/gtudhqtpbu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zdqjudy.top/gtfcwwgyip.html

[U17] Py：初始化日志
来源：http://hz.vqdsnc.cn/gtleyzjeaz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jlsjyb.cn/gtdqpmsvxk.html

[U18] Py：预编译正则
来源：http://hz.shzxlz.cn/gtcyqgjhos.html

pat = re.compile(r"\d+")
来源：http://hz.cashguo.top/gtounusoqe.html

[U19] Py：正则替换带回调
来源：http://hz.nanxinkj.top/gtmgmjxyen.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hfpthk.cn/gtvmqrgcse.html

[U20] Py：缓存函数结果
来源：http://hz.jqgfzy.top/gtbeuhqzus.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jqgfzy.top/gtyhwokqhc.html

[U21] Py：自定义上下文管理器
来源：http://hz.xinyue.icu/gtwqltxato.html

@contextlib.contextmanager
来源：http://hz.yuanzhike.top/gtyanipcpp.html

[U22] Py：矩阵转置
来源：http://hz.guowangkeji.top/gtqgufafjt.html

list(zip(*m))
来源：http://hz.xuetiantiany.cn/gtthraozio.html

[U23] Py：分块读取大文件
来源：http://hz.tanke756.top/gthvztojwn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yueranfly.top/gtdbsglllm.html

[U24] Py：路径操作
来源：http://hz.havefunace.top/gtgcideemo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtwwbhwlhe.html

[U25] Py：CSV 按字典读
来源：http://hz.zhoulong.xyz/gtezsmwhhu.html

csv.DictReader(f)
来源：http://hz.cqqwz.cn/gtfhofxoqs.html

[U26] Py：并发下载
来源：http://hz.hnxiangtu.top/gtunwxoqaa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gogol.net.cn/gtrxjomyyi.html

[U27] Py：异步 HTTP
来源：http://hz.iojbl.cn/gtmefetjue.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.svipenyu.cn/gtmjfficps.html

[U28] Py：类型别名
来源：http://hz.ydjk.org.cn/gtorgjgwep.html

UserId = int
来源：http://hz.chenzaomai.com/gtwszevygf.html

[U29] Py：属性校验
来源：http://hz.yueranfly.top/gtcyahdapq.html

@property 与 @x.setter 配合
来源：http://hz.chenzaomai.com/gtcaqcgxlp.html

[U30] Py：数据类
来源：http://hz.hammf.cn/gtysreszuc.html

@dataclass(slots=True)
来源：http://hz.zhixingplan.top/gtdmpqyzkw.html

[U31] Py：单测
来源：http://hz.daxiang520.top/gtgahqedkx.html

python -m pytest -q
来源：http://hz.shuidangran.top/gtpmfsjfoe.html

[U32] Py：代码格式化
来源：http://hz.vqdsnc.cn/gthqwqvyuz.html

ruff format . && ruff check --fix .
来源：http://hz.zhixingplan.top/gtbgaeiqll.html

[U33] Py：打包发布
来源：http://hz.shzxlz.cn/gtnbcrhhps.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shanyushiyangkeji.top/gtqqdsjsmh.html

[U34] Py：判断编码
来源：http://hz.shanyushiyangtech.top/gtudwanvbd.html

chardet.detect(raw)
来源：http://hz.hywenlv.cn/gtrqjtwgdp.html

[U35] Py：发送邮件
来源：http://hz.kuanghao11.cn/gtoitngruj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cucudq.cn/gtusikjxwl.html

[U36] Py：定时任务
来源：http://hz.hnxiangtu.top/gtvjjcjogw.html

schedule.every(10).minutes.do(job)
来源：http://hz.shangyingyoupin.top/gthvobmhrw.html

[U37] Py：读写 Excel
来源：http://hz.andypj.xyz/gtfwewyuhf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhengqikj.top/gthifixvek.html

[U38] Py：获取脚本所在目录
来源：http://hz.shangyingyoupin.top/gtanutymws.html

Path(__file__).resolve().parent
来源：http://hz.zhixingplan.top/gtdsufxylc.html

[U39] Py：判断是否在交互环境
来源：http://hz.shanyushiyangkeji.top/gtkldfaqpu.html

sys.stdout.isatty()
来源：http://hz.tian-w.cn/gtllldgyvu.html

[U40] Py：打印到标准错误
来源：http://hz.andypj.xyz/gtbcytgpjm.html

print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtsofeltsh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.nwbrower.top/gtiswdkdbg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenlongwang.top/gthkdfhpiq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jqgfzy.top/gtcsmdmaid.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hongshengwenyu.top/gtxohcoxwo.html

[U43] PHP：声明命名空间
来源：http://hz.kuanghao11.cn/gtnqxrxqhk.html

namespace App\Http;
来源：http://hz.nwbrower.top/gttlhbhpsa.html

[U44] PHP：开启严格类型
来源：http://hz.haohaochexian.top/gthgaipsrz.html

declare(strict_types=1);
来源：http://hz.yangfankeji.com/gtqliwfezh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhaomingkeji.xyz/gtrxndkelp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtnjwcflmr.html

[U46] PHP：可空类型
来源：http://hz.ydjk.org.cn/gtoxmhfllm.html

?string $name = null
来源：http://hz.yvedp.cn/gtlxzkimiq.html

[U47] PHP：联合类型
来源：http://hz.jinghuilouyu.cn/gtehgyslej.html

int|string $id
来源：http://hz.sweek.top/gtjuyhkqly.html

[U48] PHP：纯枚举
来源：http://hz.yongpay.top/gtickjdwbv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.mhx1999.top/gtsztovmqe.html

[U49] PHP：只读属性
来源：http://hz.redwolf501.top/gtxkqwwksr.html

public readonly string $name
来源：http://hz.jianghu66.top/gthqcmhkxr.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gtvapbavaj.html

public function __construct(private int $id) {}
来源：http://hz.birdmap.top/gtfstbbwvg.html

[U51] PHP：数组解构
来源：http://hz.zhoulong.xyz/gtnduiyukb.html

[$a, $b] = $arr;
来源：http://hz.shangyingyoupin.top/gtgnxhqoue.html

[U52] PHP：箭头函数
来源：http://hz.nanxinkj.top/gtaeadjxdb.html

$double = fn($x) => $x * 2;
来源：http://hz.dianchejie.cn/gtbdbhaxft.html

[U53] PHP：空合并运算符
来源：http://hz.zhijiandao.cn/gteccttwxc.html

$v = $a ?? $b ?? "default";
来源：http://hz.andypj.xyz/gtfzeqrsqz.html

[U54] PHP：空安全调用
来源：http://hz.xuetiantiany.cn/gtxvvnmnbv.html

$obj?->method()
来源：http://hz.hysaishi.cn/gthpvmapgo.html

[U55] PHP：match 表达式
来源：http://hz.zhengqikj.top/gtpipbjoyc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.fzhhl.top/gtluxzwbsw.html

[U56] PHP：命名参数
来源：http://hz.yvedp.cn/gtgwomfpzb.html

f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtvrdsuzjz.html

[U57] PHP：字符串插值
来源：http://hz.jiagoushi.top/gtrndnalpq.html

"值: {$a}"
来源：http://hz.daxiang520.top/gtsnxbhocv.html

[U58] PHP：数组三件套
来源：http://hz.chenzaomai.com/gthesvnvci.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.kuanghao11.cn/gtcnkwnmzw.html

[U59] PHP：自定义排序
来源：http://hz.pycfn.com/gtxyzcdiuw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtygpooovf.html

[U60] PHP：JSON 编解码
来源：http://hz.fzhhl.top/gtboreqqgu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenlongwang.top/gtoovvngob.html

[U61] PHP：正则
来源：http://hz.yongpay.top/gtsrevltiq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtfdiqlign.html

[U62] PHP：日期对象
来源：http://hz.0kj1m.cn/gtetstvxtr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.bjfxy.top/gtvbjogqor.html

[U63] PHP：文件读写
来源：http://hz.jqgufenzy.top/gtvzcrrqip.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cucudq.cn/gtmnqbymod.html

[U64] PHP：目录遍历
来源：http://hz.sufxvd.cn/gtesdqyfuq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhongyouzk.top/gtyxsumxpj.html

[U65] PHP：会话
来源：http://hz.shanyushiyangkeji.top/gtdxnvyvdu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.nwbrower.top/gtuozzjmli.html

[U66] PHP：设置 Cookie
来源：http://hz.sysykeji.top/gtwauhiaab.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.wangshuangyany.cn/gtbrdjkdce.html

[U67] PHP：处理文件上传
来源：http://hz.quarkkingdee.top/gtghodvjyh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.fengsongda.top/gtmuumiaev.html

[U68] PHP：PDO 连接
来源：http://hz.guannengcc.top/gtytwrgzsv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yvedp.cn/gtbzaetfrd.html

[U69] PHP：PDO 预处理
来源：http://hz.jiagoushi.top/gtqwexrkyi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gzhubu.top/gtchtsybbt.html

[U70] PHP：PDO 事务
来源：http://hz.jlsjyb.cn/gtnljhjylv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.dashuyun.cn/gtriuffnqn.html

[U71] PHP：抛出异常
来源：http://hz.jinghuilouyu.cn/gtqdrayjkq.html

throw new RuntimeException("失败", 500);
来源：http://hz.gogol.net.cn/gtrympzvaf.html

[U72] PHP：写错误日志
来源：http://hz.gaohongyu789.top/gtnxhoeeuq.html

error_log("失败: " . $e->getMessage());
来源：http://hz.bjfxy.top/gtantjgbpe.html

[U73] PHP：读取 ini 配置
来源：http://hz.cqqwz.cn/gttpugtmfj.html

parse_ini_file("config.ini", true)
来源：http://hz.yueranfly.top/gtxcnjwqlk.html

[U74] PHP：读取环境变量
来源：http://hz.aibaodan.cn/gtxnxzcpue.html

getenv("APP_ENV") ?: "production"
来源：http://hz.havefunace.top/gthjuuehnt.html

[U75] PHP：依赖注入
来源：http://hz.xziqi.cn/gtwuzwffta.html

composer require psr/container
来源：http://hz.pycfn.com/gthbdalarh.html

[U76] PHP：简单路由
来源：http://hz.zhoulong.xyz/gtzdnslraw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhengqikj.top/gtuxxftskh.html

[U77] PHP：模板渲染
来源：http://hz.ybcxt.top/gtrwcqzwxd.html

composer require twig/twig
来源：http://hz.cucudq.cn/gtrkpqnbmp.html

[U78] PHP：单元测试
来源：http://hz.yuxming.cn/gtlbmxzeeq.html

composer require --dev phpunit/phpunit
来源：http://hz.havefunace.top/gtcobuncez.html

[U79] PHP：静态分析
来源：http://hz.shangyingyoupin.top/gtxikjxzvu.html

composer require --dev phpstan/phpstan
来源：http://hz.hywenlv.cn/gtalhghcse.html

[U80] PHP：代码规范修复
来源：http://hz.chenjidiqi.icu/gtmgiqhhfi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xylfe.cn/gtxbrejtds.html

[U81] JS：初始化项目
来源：http://hz.xziqi.cn/gtbxdrraob.html

npm init -y;  npm i express
来源：http://hz.hongshengwenyu.top/gtezjlbxuq.html

[U82] JS：package.json 脚本
来源：http://hz.xingfuxueyuan.xyz/gtngqbjrxy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zycfv.cn/gtxxqxwubd.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinqigfzy.top/gtfluvgdzc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gzhubu.top/gtnpcdunig.html

[U84] JS：CommonJS 写法
来源：http://hz.zycfv.cn/gtfuxcnfcg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinqigufen.top/gtamncrcmd.html

[U85] JS：可选链
来源：http://hz.tianlin.xyz/gtyijgmrru.html

a?.b?.c
来源：http://hz.ybcxt.top/gtibpvpwkq.html

[U86] JS：空值合并
来源：http://hz.birdmap.top/gtgjcqwckn.html

a ?? b
来源：http://hz.zhaomingkeji.xyz/gtcntfntvb.html

[U87] JS：解构默认值
来源：http://hz.yj20258.top/gtfuxwxryj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sxryk.cn/gtxammzvur.html

[U88] JS：对象展开合并
来源：http://hz.pycfn.com/gtnongbydn.html

{ ...a, ...b }
来源：http://hz.xuetiantiany.cn/gtmqyxpnel.html

[U89] JS：数组去重
来源：http://hz.bjfxy.top/gtgbtjnjif.html

[...new Set(arr)]
来源：http://hz.tianlin.xyz/gtirtvfjji.html

[U90] JS：数字数组排序
来源：http://hz.kuanghao11.cn/gtepmtihqv.html

[...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gtivagduzm.html

[U91] JS：对象键值遍历
来源：http://hz.wangdashe.top/gtekcbswfh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhongyouzk.top/gtlqjajpyq.html

[U92] JS：深拷贝
来源：http://hz.pengpengdd.cyou/gttlbjcbfq.html

structuredClone(obj)
来源：http://hz.yueranfly.top/gtrvzoynda.html

[U93] JS：模板字符串
来源：http://hz.zhengqikj.top/gtewkaohmo.html

`共 ${n} 条`
来源：http://hz.aibaodan.cn/gtlsqfbcyt.html

[U94] JS：箭头函数
来源：http://hz.chenjidiqi.icu/gtylqscakj.html

const double = x => x * 2;
来源：http://hz.yanxiufei.cn/gtcrvsorxn.html

[U95] JS：Promise 包装
来源：http://hz.jinqigufen.top/gtwgvjivtb.html

new Promise((resolve, reject) => {})
来源：http://hz.yueranfly.top/gtokjmdsxr.html

[U96] JS：async/await 与异常
来源：http://hz.hnqzz.top/gtzqrnjldn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.pycfn.com/gtawyfcutn.html

[U97] JS：并发请求
来源：http://hz.jinqigfzy.top/gtpbklcoiq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtsuglvxot.html

[U98] JS：fetch 带 JSON
来源：http://hz.52xcode.cn/gtfrldlghh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xylfe.cn/gtpyfmrrwy.html

[U99] JS：事件监听
来源：http://hz.52xcode.cn/gtlchlzidr.html

el.addEventListener("click", e => {})
来源：http://hz.gzhubu.top/gtvqcmulwh.html

[U100] JS：DOM 查询
来源：http://hz.0kj1m.cn/gtgjuuwwgi.html

document.querySelector(".item")
来源：http://hz.hfpthk.cn/gtsrffojng.html

[U101] JS：classList 操作
来源：http://hz.pycfn.com/gtmoavrblp.html

el.classList.toggle("active")
来源：http://hz.dianchejie.cn/gtfmeqqjlr.html

[U102] JS：本地存储
来源：http://hz.wangshuangyany.cn/gtjxygcnao.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xuetiantiany.cn/gtxnojnlwn.html

[U103] JS：定时器
来源：http://hz.ppjwa.cn/gtiujmegjv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.andypj.xyz/gtovynsuww.html

[U104] JS：防抖
来源：http://hz.birdmap.top/gtzxaknhhn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtlgilclvu.html

[U105] JS：节流
来源：http://hz.yonumen.top/gtqsgzmpta.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yueranfly.top/gtniwgedpi.html

[U106] JS：日期格式化
来源：http://hz.jqgfzy.top/gtlibmparg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yanxiufei.cn/gtbwyspvwf.html

[U107] JS：数字千分位
来源：http://hz.jinghuilouyu.cn/gtnttuwuxy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ydzc1.top/gtuofwoxgo.html

[U108] JS：随机整数
来源：http://hz.andypj.xyz/gtjnpluqvy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yonumen.top/gtesqieqck.html

[U109] JS：数组分组
来源：http://hz.cucudq.cn/gtadcsxzoe.html

Object.groupBy(arr, x => x.type)
来源：http://hz.kuanghao11.cn/gtufaiqhua.html

[U110] JS：数组分块
来源：http://hz.birdmap.top/gtnyuewxgx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.vqdsnc.cn/gtsxolwqxo.html

[U111] JS：对象转 Map
来源：http://hz.xingfuxueyuan.xyz/gtoknirqso.html

new Map(Object.entries(obj))
来源：http://hz.xziqi.cn/gtsywvuknn.html

[U112] JS：字符串补位
来源：http://hz.cdnleiting.top/gtsummlomj.html

"7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtarnfkcex.html

[U113] JS：正则替换全部
来源：http://hz.ivvv.top/gttubhsusx.html

s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtipyoucmg.html

[U114] JS：JSON 深比较
来源：http://hz.daria6918.cn/gtdekyqatz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhengqikj.top/gtekgdbakr.html

[U115] JS：生成 UUID
来源：http://hz.xuanzx.com/gtepjtejeb.html

crypto.randomUUID()
来源：http://hz.havefunace.top/gtaxfbbtgr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yanxiufei.cn/gtafazvpmf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shuidangran.top/gtgowjljou.html

[U117] JS：单元测试
来源：http://hz.haohaochexian.top/gtrxskfnrg.html

npm i -D vitest;  npx vitest
来源：http://hz.shuidangran.top/gtrmfqhxye.html

[U118] JS：开发服务器
来源：http://hz.0kj1m.cn/gtkvclceql.html

npm i -D vite;  npx vite
来源：http://hz.hnqzz.top/gtclxrjzuj.html

[U119] JS：生产构建
来源：http://hz.svipenyu.cn/gthwrcwkvr.html

npx vite build
来源：http://hz.zycfv.cn/gtdhnymemh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenlongwang.top/gtcpkexmao.html

import.meta.env.VITE_API_URL
来源：http://hz.gotoacloud.top/gtuqseatud.html

================================================================================
来源：http://hz.yueranfly.top/gtqozizanv.html

统计汇总
来源：http://hz.fzhhl.top/gttzevqcwc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbzjoptmf.html

按语言统计（条）：
来源：http://hz.quarkkingdee.top/gtrfnxowek.html

Python ......... 252
来源：http://hz.yonumen.top/gtcbnwyncd.html

PHP ............ 252
来源：http://hz.zycfv.cn/gtjgwuglda.html

JavaScript ..... 252
来源：http://hz.quarkkingdee.top/gtawjzmtuk.html

TypeScript ..... 212
来源：http://hz.jyoumei.cn/gtnpmrtloz.html

Java ........... 212
来源：http://hz.jinghuilouyu.cn/gtsiyyqxhz.html

Go ............. 212
来源：http://hz.mhx1999.top/gtqntvzssm.html

Ruby ........... 212
来源：http://hz.jyoumei.cn/gtajfnutzf.html

C# ............. 212
来源：http://hz.ybcxt.top/gtvutpojct.html

C .............. 30
来源：http://hz.svipenyu.cn/gthgizmdpq.html

C++ ............ 30
来源：http://hz.hywenlv.cn/gtjhhzzafv.html

SQL ............ 90
来源：http://hz.shuidangran.top/gtsksubvnx.html

Bash ........... 80
来源：http://hz.shanyushiyangtech.top/gtujvwcktu.html

Kotlin ......... 15
来源：http://hz.guowangkeji.top/gtbjisxogc.html

Swift .......... 15
来源：http://hz.hnxiangtu.top/gtehmtclvt.html

Lua ............ 10
来源：http://hz.ehwqpu.com/gtrmoykrsj.html

Perl ........... 10
来源：http://hz.zhaomingkeji.xyz/gtfhdmzaxm.html

Scala .......... 10
来源：http://hz.hnxiangtu.top/gtwcuvewfb.html

------------------------------------
来源：http://hz.jqgfzy.top/gtnnlminar.html

合计 ........... 2106 条
来源：http://hz.nanxinkj.top/gtggolsinb.html

按章节统计：
来源：http://hz.316326.xyz/gtnclxylke.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtlyenacbx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gtgwahujtl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gthoqzkbcp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhoulong.xyz/gtufvymqss.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xziqi.cn/gtppljkpwm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinyuanbaomall.cn/gtkiarjwvt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtsejpzsji.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shuidangran.top/gtqyllaeuj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ydjk.org.cn/gtaaglmolk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.fzhhl.top/gtysgmeqew.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtfcgsdlux.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtytofnpnx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtifwrpjag.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yonumen.top/gtlchicjbx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yvedp.cn/gtwvcbeebr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtvitprotl.html

Q SQL 专题                              90
来源：http://hz.chenzaomai.com/gtapsgtgeh.html

R Bash 专题                             80
来源：http://hz.zhoulong.xyz/gtgnbvcmvg.html

S C / C++ 专题                          60
来源：http://hz.shanyushiyangkeji.top/gtijjuxqxb.html

T 其他语言补充                          60
来源：http://hz.xziqi.cn/gtsczayfoc.html


<!-- 参考信息 -->