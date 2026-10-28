代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.zdqjudy.top/gttefysjhm.html

[T55] Scala：集合过滤
来源：http://hz.kuanghao11.cn/gtylrbiict.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.aizwys.cn/gthsunfrii.html

[T56] Scala：样例类
来源：http://hz.cheryme.top/gtwjcpkivh.html

case class User(name: String, age: Int)
来源：http://hz.cdnleiting.top/gtnqwchbkc.html

[T57] Scala：模式匹配
来源：http://hz.gaohongyu789.top/gtnxkxmmsq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yanxiufei.cn/gtzsdkvcuh.html

[T58] Scala：函数定义
来源：http://hz.gotoacloud.top/gtvsyxyefz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgufenzy.top/gtvvzzcqau.html

[T59] Scala：循环
来源：http://hz.xuetiantiany.cn/gtuspnscxc.html

for (i <- 1 to 10) println(i)
来源：http://hz.aizwys.cn/gtnqxfpsyy.html

[T60] Scala：折叠
来源：http://hz.iojbl.cn/gtgffileeo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangkeji.top/gtmuirbrex.html

================================================================================
来源：http://hz.316326.xyz/gtgddniyck.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.fengsongda.top/gtaqqhylny.html

================================================================================
来源：http://hz.sweek.top/gtuarnpycy.html

[U01] Py：创建虚拟环境
来源：http://hz.hongshengwenyu.top/gthrgkvffo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.52xcode.cn/gtbgelpeec.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhongyouzk.top/gthvkduedf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jiagoushi.top/gthdexxxgw.html

[U03] Py：加载 .env 配置
来源：http://hz.mhx1999.top/gthugwkqdo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xinyue.icu/gtdefdbjmr.html

[U04] Py：变量调试打印
来源：http://hz.zhijiandao.cn/gtcjepkiaa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.daxiang520.top/gtmjowludm.html

[U05] Py：列表去重且保序
来源：http://hz.cqqwz.cn/gtprgeztjp.html

list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gtkmrrvfev.html

[U06] Py：合并两个字典
来源：http://hz.zhoulong.xyz/gtafvauuct.html

{**a, **b}
来源：http://hz.yvedp.cn/gtgcqigvtc.html

[U07] Py：反转字典键值
来源：http://hz.ivvv.top/gtrcpgndxo.html

{v: k for k, v in d.items()}
来源：http://hz.sysykeji.top/gtaytizzrn.html

[U08] Py：展平二维列表
来源：http://hz.fengsongda.top/gtolfgzqgl.html

[y for x in nested for y in x]
来源：http://hz.dianchejie.cn/gtcdemtpfy.html

[U09] Py：字典取最大值的键
来源：http://hz.shzxlz.cn/gtugvyqbdb.html

max(d, key=d.get)
来源：http://hz.ppjwa.cn/gtlhgahgrn.html

[U10] Py：按值排序字典
来源：http://hz.ydjk.org.cn/gtzmjveduc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.mhx1999.top/gtyhnvksen.html

[U11] Py：生成器表达式
来源：http://hz.bjfxy.top/gtyqrkcmdt.html

(x * 2 for x in arr)
来源：http://hz.hfpthk.cn/gtwfvcubmh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.birdmap.top/gtdmvjexbb.html

Counter(arr).most_common(3)
来源：http://hz.yonumen.top/gtjkmvjwex.html

[U13] Py：固定长度队列
来源：http://hz.ehwqpu.com/gthhzaohfw.html

deque(maxlen=10)
来源：http://hz.jinqigfzy.top/gtsrqgdkpq.html

[U14] Py：分组收集到列表
来源：http://hz.gzhubu.top/gtaxeidvmz.html

defaultdict(list)
来源：http://hz.chenjidiqi.icu/gtvhnenrjl.html

[U15] Py：高精度计时
来源：http://hz.aizwys.cn/gtvshcvlla.html

t = time.perf_counter()
来源：http://hz.shzxlz.cn/gtganmfzmw.html

[U16] Py：命令行参数解析
来源：http://hz.ehwqpu.com/gttkiergrg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtwufsbfhp.html

[U17] Py：初始化日志
来源：http://hz.0kj1m.cn/gtufpmbopd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fengsongda.top/gtkkbpxkqj.html

[U18] Py：预编译正则
来源：http://hz.ehwqpu.com/gtsdpeyzli.html

pat = re.compile(r"\d+")
来源：http://hz.sufxvd.cn/gtkntgrydz.html

[U19] Py：正则替换带回调
来源：http://hz.nanxinkj.top/gtvinyuqbc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.fengsongda.top/gtvxtjldxu.html

[U20] Py：缓存函数结果
来源：http://hz.jqgufenzy.top/gtsplrlnrc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dianchejie.cn/gtewhntjor.html

[U21] Py：自定义上下文管理器
来源：http://hz.hnqzz.top/gtjwcufxqu.html

@contextlib.contextmanager
来源：http://hz.cdnleiting.top/gtrljomxlb.html

[U22] Py：矩阵转置
来源：http://hz.jqgfzy.top/gtsufciapx.html

list(zip(*m))
来源：http://hz.guannengcc.top/gtkarzxvcg.html

[U23] Py：分块读取大文件
来源：http://hz.svipenyu.cn/gthfxtxiyl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gotoacloud.top/gtvowfczze.html

[U24] Py：路径操作
来源：http://hz.smart0.xyz/gtrundotgz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hywenlv.cn/gtacclqtrv.html

[U25] Py：CSV 按字典读
来源：http://hz.dianchejie.cn/gtqzdberyy.html

csv.DictReader(f)
来源：http://hz.shanyushiyangtech.top/gtacguoret.html

[U26] Py：并发下载
来源：http://hz.haohaochexian.top/gtxmojweoc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daria6918.cn/gtydehtyse.html

[U27] Py：异步 HTTP
来源：http://hz.meibo888.top/gtskdxlajf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gzhubu.top/gtspqjntru.html

[U28] Py：类型别名
来源：http://hz.nwbrower.top/gtjdwvfqbk.html

UserId = int
来源：http://hz.tian-w.cn/gtskfmefln.html

[U29] Py：属性校验
来源：http://hz.jinghuilouyu.cn/gtjldiakxx.html

@property 与 @x.setter 配合
来源：http://hz.dianchejie.cn/gtutguvwjd.html

[U30] Py：数据类
来源：http://hz.gzhubu.top/gtcrgmhrax.html

@dataclass(slots=True)
来源：http://hz.ywan-chungtsiang.top/gtapuzojih.html

[U31] Py：单测
来源：http://hz.ppjwa.cn/gtruxeweqq.html

python -m pytest -q
来源：http://hz.hammf.cn/gtgzhowfwm.html

[U32] Py：代码格式化
来源：http://hz.hysaishi.cn/gtboljaogu.html

ruff format . && ruff check --fix .
来源：http://hz.hfpthk.cn/gtezwicyah.html

[U33] Py：打包发布
来源：http://hz.fzhhl.top/gtblfxqrwf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ppjwa.cn/gtsmxnxaxm.html

[U34] Py：判断编码
来源：http://hz.guannengcc.top/gtujawzbec.html

chardet.detect(raw)
来源：http://hz.yongpay.top/gtjmpsdozm.html

[U35] Py：发送邮件
来源：http://hz.pycfn.com/gtedctbgrb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shuidangran.top/gtogcgscio.html

[U36] Py：定时任务
来源：http://hz.sysykeji.top/gtsfxejxhw.html

schedule.every(10).minutes.do(job)
来源：http://hz.svipenyu.cn/gtbhabpgvb.html

[U37] Py：读写 Excel
来源：http://hz.yueranfly.top/gtsltqfzgg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinghuilouyu.cn/gtgymhriqw.html

[U38] Py：获取脚本所在目录
来源：http://hz.fengsongda.top/gtfankwlmd.html

Path(__file__).resolve().parent
来源：http://hz.52xcode.cn/gtazjzonbx.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhixingplan.top/gtrwglbhdv.html

sys.stdout.isatty()
来源：http://hz.zhiwuduotai.top/gtdbfnollq.html

[U40] Py：打印到标准错误
来源：http://hz.xziqi.cn/gtznxruacx.html

print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtcsajbxtw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ybcxt.top/gtxdgfcorg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.iojbl.cn/gtuktujbdu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yongpay.top/gtocktvdie.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.daxiang520.top/gtyqdmnfuc.html

[U43] PHP：声明命名空间
来源：http://hz.pycfn.com/gtftemuzxm.html

namespace App\Http;
来源：http://hz.zhixingplan.top/gtplxitaaj.html

[U44] PHP：开启严格类型
来源：http://hz.wangdashe.top/gtgxxuawya.html

declare(strict_types=1);
来源：http://hz.shanyushiyangtech.top/gtohrwjtaw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhoulong.xyz/gtdpygfozz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtekdabpit.html

[U46] PHP：可空类型
来源：http://hz.aizwys.cn/gtkuqilewc.html

?string $name = null
来源：http://hz.zhijiandao.cn/gtmowwfqud.html

[U47] PHP：联合类型
来源：http://hz.jianghu66.top/gtdzgbtqqy.html

int|string $id
来源：http://hz.svipenyu.cn/gtkkwlhzet.html

[U48] PHP：纯枚举
来源：http://hz.9152youxi.cn/gtzbvxsvcz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zycfv.cn/gtcbahamda.html

[U49] PHP：只读属性
来源：http://hz.dashuyun.cn/gtlyqamyro.html

public readonly string $name
来源：http://hz.yonumen.top/gtazwovfkg.html

[U50] PHP：构造器属性提升
来源：http://hz.hnqzz.top/gtnbrpdbzz.html

public function __construct(private int $id) {}
来源：http://hz.cucudq.cn/gtwgueduyz.html

[U51] PHP：数组解构
来源：http://hz.quarkkingdee.top/gtvshcpgei.html

[$a, $b] = $arr;
来源：http://hz.hfpthk.cn/gtukskarxc.html

[U52] PHP：箭头函数
来源：http://hz.ppjwa.cn/gtwzzekjrk.html

$double = fn($x) => $x * 2;
来源：http://hz.9152youxi.cn/gtzzlolpwm.html

[U53] PHP：空合并运算符
来源：http://hz.zycfv.cn/gtmpfozirr.html

$v = $a ?? $b ?? "default";
来源：http://hz.xziqi.cn/gtevmtqzwy.html

[U54] PHP：空安全调用
来源：http://hz.aizwys.cn/gtebkdtfpa.html

$obj?->method()
来源：http://hz.birdmap.top/gtrptmznms.html

[U55] PHP：match 表达式
来源：http://hz.shzxlz.cn/gtxjqlbadg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yongpay.top/gthzjpmkjy.html

[U56] PHP：命名参数
来源：http://hz.smart0.xyz/gtqihbbknw.html

f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtsleznpqm.html

[U57] PHP：字符串插值
来源：http://hz.cucudq.cn/gtdzasewch.html

"值: {$a}"
来源：http://hz.wangdashe.top/gtoqujrttv.html

[U58] PHP：数组三件套
来源：http://hz.ywan-chungtsiang.top/gtnikwspww.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shzxlz.cn/gtdtfjakll.html

[U59] PHP：自定义排序
来源：http://hz.sxryk.cn/gttwvkllby.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jlsjyb.cn/gtwfucvbqk.html

[U60] PHP：JSON 编解码
来源：http://hz.snrcjt.cn/gtbhsgfdoh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.aizwys.cn/gtjpjibiun.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gttmbwdfno.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.smart0.xyz/gtavaqjnbr.html

[U62] PHP：日期对象
来源：http://hz.yonumen.top/gthhbxtquu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yanxiufei.cn/gtkkvzoubq.html

[U63] PHP：文件读写
来源：http://hz.mhx1999.top/gtknmjcqyz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jlsjyb.cn/gtzdcmudgp.html

[U64] PHP：目录遍历
来源：http://hz.chenlongwang.top/gtwodcnfvh.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hongshengwenyu.top/gtrjomqoyv.html

[U65] PHP：会话
来源：http://hz.ybcxt.top/gtwljboiao.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sufxvd.cn/gtclxwzkif.html

[U66] PHP：设置 Cookie
来源：http://hz.xuetiantiany.cn/gtwaxzxdql.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.nwbrower.top/gtrpzvafjd.html

[U67] PHP：处理文件上传
来源：http://hz.jinghuilouyu.cn/gtvdabeopa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shanyushiyangtech.top/gtvatiauxt.html

[U68] PHP：PDO 连接
来源：http://hz.guowangkeji.top/gtftiohfqx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.snrcjt.cn/gtzopgfwiy.html

[U69] PHP：PDO 预处理
来源：http://hz.wangdashe.top/gtiwbrpwer.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hongshengwenyu.top/gtapuuuhvx.html

[U70] PHP：PDO 事务
来源：http://hz.quarkkingdee.top/gtouxleqgz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.mhx1999.top/gtpzbmunnz.html

[U71] PHP：抛出异常
来源：http://hz.ywan-chungtsiang.top/gtjoqdibok.html

throw new RuntimeException("失败", 500);
来源：http://hz.yueranfly.top/gtmqulrrty.html

[U72] PHP：写错误日志
来源：http://hz.wangdashe.top/gttsbxzomy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.redwolf501.top/gtuxlnvzlt.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhoulong.xyz/gtuvzqxxhe.html

parse_ini_file("config.ini", true)
来源：http://hz.feifeiyinyue.top/gtvwwxoazr.html

[U74] PHP：读取环境变量
来源：http://hz.zhijiandao.cn/gtgscqciib.html

getenv("APP_ENV") ?: "production"
来源：http://hz.nanxuanxn.top/gtrqbwzsdx.html

[U75] PHP：依赖注入
来源：http://hz.xuetiantiany.cn/gtieczrpvc.html

composer require psr/container
来源：http://hz.havefunace.top/gtdhuhixos.html

[U76] PHP：简单路由
来源：http://hz.cheryme.top/gthmpkzmjg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhongyouzk.top/gtquwmvxic.html

[U77] PHP：模板渲染
来源：http://hz.zhiwuduotai.top/gtakmfwpat.html

composer require twig/twig
来源：http://hz.haohaochexian.top/gtqtrnjlyl.html

[U78] PHP：单元测试
来源：http://hz.ppjwa.cn/gtnpatriuz.html

composer require --dev phpunit/phpunit
来源：http://hz.gotoacloud.top/gtcpfwmgqs.html

[U79] PHP：静态分析
来源：http://hz.tian-w.cn/gtdmnisdrv.html

composer require --dev phpstan/phpstan
来源：http://hz.hnxiangtu.top/gtpygyiwdr.html

[U80] PHP：代码规范修复
来源：http://hz.yuanzhike.top/gtexdfgswc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hammf.cn/gtwizdsgqf.html

[U81] JS：初始化项目
来源：http://hz.shuidangran.top/gtgvrgudcv.html

npm init -y;  npm i express
来源：http://hz.kuanghao11.cn/gtwtmrbqum.html

[U82] JS：package.json 脚本
来源：http://hz.chenzaomai.com/gtpqvkgacj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.wangdashe.top/gtsaysornj.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhiwuduotai.top/gtnrxkolwq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.mhx1999.top/gtctdrvlyj.html

[U84] JS：CommonJS 写法
来源：http://hz.yongpay.top/gtwxjxlofs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.snrcjt.cn/gtrznkxivc.html

[U85] JS：可选链
来源：http://hz.yvedp.cn/gtxkembjeu.html

a?.b?.c
来源：http://hz.tian-w.cn/gtdilunxec.html

[U86] JS：空值合并
来源：http://hz.shanyushiyangkeji.top/gtyhxpdfif.html

a ?? b
来源：http://hz.xingfuxueyuan.xyz/gtlqfnlmxn.html

[U87] JS：解构默认值
来源：http://hz.zdqjudy.top/gtddpiobjj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jiagoushi.top/gtbydacjft.html

[U88] JS：对象展开合并
来源：http://hz.kuanghao11.cn/gtlpqmyktz.html

{ ...a, ...b }
来源：http://hz.jianghu66.top/gttbodzjpa.html

[U89] JS：数组去重
来源：http://hz.zhiwuduotai.top/gtpidnonmz.html

[...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtoaarcvaf.html

[U90] JS：数字数组排序
来源：http://hz.zhongyouzk.top/gtewvsabxq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gttzxhyvdz.html

[U91] JS：对象键值遍历
来源：http://hz.xziqi.cn/gtfislhnjc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.fengsongda.top/gtyavcvxca.html

[U92] JS：深拷贝
来源：http://hz.sysykeji.top/gtvymtbzal.html

structuredClone(obj)
来源：http://hz.yj202588.top/gtbiqtbsgy.html

[U93] JS：模板字符串
来源：http://hz.jinghuilouyu.cn/gtpccanicj.html

`共 ${n} 条`
来源：http://hz.guannengcc.top/gtsruoxvwz.html

[U94] JS：箭头函数
来源：http://hz.hywenlv.cn/gtzyzfounw.html

const double = x => x * 2;
来源：http://hz.hongshengwenyu.top/gtutlejbqh.html

[U95] JS：Promise 包装
来源：http://hz.jiagoushi.top/gtxmpbouqy.html

new Promise((resolve, reject) => {})
来源：http://hz.hammf.cn/gtofzwzxok.html

[U96] JS：async/await 与异常
来源：http://hz.cheryme.top/gtdgbzntob.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtmmdnbjpp.html

[U97] JS：并发请求
来源：http://hz.tanke756.top/gtfrbqzjpq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtqfsgocba.html

[U98] JS：fetch 带 JSON
来源：http://hz.hysaishi.cn/gtzrmeegdj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yonumen.top/gtdqeqftkw.html

[U99] JS：事件监听
来源：http://hz.redwolf501.top/gtyepugvbr.html

el.addEventListener("click", e => {})
来源：http://hz.shanyushiyangtech.top/gtevvhuftw.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtxwmfgcgo.html

document.querySelector(".item")
来源：http://hz.daxiang520.top/gtuowsmrit.html

[U101] JS：classList 操作
来源：http://hz.wangshuangyany.cn/gtjaaijkog.html

el.classList.toggle("active")
来源：http://hz.sysykeji.top/gthneoupzv.html

[U102] JS：本地存储
来源：http://hz.sweek.top/gtoxqulszt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shzxlz.cn/gtyzwtaffk.html

[U103] JS：定时器
来源：http://hz.hysaishi.cn/gtrageshpr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.tanke756.top/gtpaygmwoy.html

[U104] JS：防抖
来源：http://hz.jinghuilouyu.cn/gtoujealjp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtuzolnumk.html

[U105] JS：节流
来源：http://hz.ybcxt.top/gtqnsefbsc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhengqikj.top/gtjeyjfogr.html

[U106] JS：日期格式化
来源：http://hz.316326.xyz/gtlvbpfckw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.9152youxi.cn/gtagwzegrq.html

[U107] JS：数字千分位
来源：http://hz.zhixingplan.top/gtmftsxxmh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.316326.xyz/gtnxcuewih.html

[U108] JS：随机整数
来源：http://hz.yanxiufei.cn/gtqjfpfdmp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cashguo.top/gtmgqdlzwy.html

[U109] JS：数组分组
来源：http://hz.jinyuanbaomall.cn/gtblmcrgiu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtsjkmmgoy.html

[U110] JS：数组分块
来源：http://hz.dianchejie.cn/gtrxcybger.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tanke756.top/gtvyndjsnl.html

[U111] JS：对象转 Map
来源：http://hz.yj20258.top/gtsdtwftbr.html

new Map(Object.entries(obj))
来源：http://hz.shanyushiyangtech.top/gthbeijmne.html

[U112] JS：字符串补位
来源：http://hz.aibaodan.cn/gtjmuefqts.html

"7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtwkrfumvv.html

[U113] JS：正则替换全部
来源：http://hz.jinyuanbaomall.cn/gtvqfzeoar.html

s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtnfojsfun.html

[U114] JS：JSON 深比较
来源：http://hz.jlsjyb.cn/gtiptoqrrr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtlrqxdfkb.html

[U115] JS：生成 UUID
来源：http://hz.ydzc1.top/gtprserisk.html

crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtisfxddtw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yangfankeji.com/gtxixmnbbb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xuetiantiany.cn/gtckgblmin.html

[U117] JS：单元测试
来源：http://hz.yongpay.top/gtifpsagps.html

npm i -D vitest;  npx vitest
来源：http://hz.dashuyun.cn/gtvdrqebqo.html

[U118] JS：开发服务器
来源：http://hz.ehwqpu.com/gtcptbctum.html

npm i -D vite;  npx vite
来源：http://hz.zhaomingkeji.xyz/gttaziwcxr.html

[U119] JS：生产构建
来源：http://hz.sxryk.cn/gtsbgaykoq.html

npx vite build
来源：http://hz.dashuyun.cn/gttqxihesv.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.nwbrower.top/gtjwonpxsi.html

import.meta.env.VITE_API_URL
来源：http://hz.ydjk.org.cn/gtbddhibda.html

================================================================================
来源：http://hz.hammf.cn/gtjqxlrnac.html

统计汇总
来源：http://hz.andypj.xyz/gtpweexobb.html

================================================================================
来源：http://hz.jyoumei.cn/gtxsdqaatd.html

按语言统计（条）：
来源：http://hz.vqdsnc.cn/gtvyxmqejr.html

Python ......... 252
来源：http://hz.ydjk.org.cn/gtdduksujx.html

PHP ............ 252
来源：http://hz.gaohongyu789.top/gtfwadmldj.html

JavaScript ..... 252
来源：http://hz.wangshuangyany.cn/gtsjlbtuni.html

TypeScript ..... 212
来源：http://hz.sufxvd.cn/gtdzvqglnj.html

Java ........... 212
来源：http://hz.hnxiangtu.top/gtswizonuf.html

Go ............. 212
来源：http://hz.nwbrower.top/gtjacqhtbw.html

Ruby ........... 212
来源：http://hz.zhongyouzk.top/gtqxptjpum.html

C# ............. 212
来源：http://hz.sweek.top/gthxlchjsy.html

C .............. 30
来源：http://hz.yuxming.cn/gtizlcryyf.html

C++ ............ 30
来源：http://hz.sufxvd.cn/gtpwztuqsg.html

SQL ............ 90
来源：http://hz.xinyue.icu/gtvtwjpecf.html

Bash ........... 80
来源：http://hz.andypj.xyz/gtmanwgdrs.html

Kotlin ......... 15
来源：http://hz.sweek.top/gtkwwbvcei.html

Swift .......... 15
来源：http://hz.xinyue.icu/gtmdtiblht.html

Lua ............ 10
来源：http://hz.jinghuilouyu.cn/gthmvhpiqz.html

Perl ........... 10
来源：http://hz.yj202588.top/gtiewrrtcq.html

Scala .......... 10
来源：http://hz.pengpengdd.cyou/gtokizwoio.html

------------------------------------
来源：http://hz.iojbl.cn/gtfuahbkyy.html

合计 ........... 2106 条
来源：http://hz.fengsongda.top/gtymaoniey.html

按章节统计：
来源：http://hz.sweek.top/gtnodbflba.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.9152youxi.cn/gtsiivfdbt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.wangshuangyany.cn/gtfvfsvdqy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.52xcode.cn/gtsslbfrqs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cqqwz.cn/gteaazbuxt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shanyushiyangkeji.top/gtgkzwtbkl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.quarkkingdee.top/gtrbqeqnvb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtgmxexbvc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sysykeji.top/gtqyuwbzxh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtaurjaluo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yvedp.cn/gtoxsyixei.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtccpogrcv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hammf.cn/gtilnaruzu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gthigtbtzv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shzxlz.cn/gtjhalzoxd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.dashuyun.cn/gtuzamokja.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gteclbombn.html

Q SQL 专题                              90
来源：http://hz.tanke756.top/gtgpzlknel.html

R Bash 专题                             80
来源：http://hz.yongpay.top/gtpngskfdf.html

S C / C++ 专题                          60
来源：http://hz.shanyushiyangkeji.top/gtwajuyfej.html

T 其他语言补充                          60
来源：http://hz.gzhubu.top/gtffjqibkq.html


<!-- 参考信息 -->