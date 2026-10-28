代发 wailian999

case class User(name: String, age: Int)
来源：http://hz.sufxvd.cn/gtxpealtai.html

[T57] Scala：模式匹配
来源：http://hz.ppjwa.cn/gtznshovij.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hfpthk.cn/gtbyjwtibp.html

[T58] Scala：函数定义
来源：http://hz.pycfn.com/gttkiuvsui.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.feifeiyinyue.top/gtsbmbumdi.html

[T59] Scala：循环
来源：http://hz.ppjwa.cn/gtsmljlhtu.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj20258.top/gttchlarfa.html

[T60] Scala：折叠
来源：http://hz.gzhubu.top/gtpnjcqjen.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.quarkkingdee.top/gtqdazxspr.html

================================================================================
来源：http://hz.jqgfzy.top/gtuqchyovh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtyaavjxna.html

================================================================================
来源：http://hz.yuxming.cn/gtgpaxthby.html

[U01] Py：创建虚拟环境
来源：http://hz.aibaodan.cn/gtnczzypuo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.snrcjt.cn/gtgjruqcdy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sysykeji.top/gtavolefhu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gtasbbgsxt.html

[U03] Py：加载 .env 配置
来源：http://hz.52xcode.cn/gtqkgybbzo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yanxiufei.cn/gtiqwlhuxd.html

[U04] Py：变量调试打印
来源：http://hz.hywenlv.cn/gtkjtmxfsa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258888.top/gtkxzrrkqz.html

[U05] Py：列表去重且保序
来源：http://hz.tanke756.top/gtvmdkuicd.html

list(dict.fromkeys(arr))
来源：http://hz.52xcode.cn/gtatnlrskw.html

[U06] Py：合并两个字典
来源：http://hz.aizwys.cn/gtbcszipol.html

{**a, **b}
来源：http://hz.ppjwa.cn/gtngnvfaja.html

[U07] Py：反转字典键值
来源：http://hz.fzhhl.top/gthsjcrdwm.html

{v: k for k, v in d.items()}
来源：http://hz.hnqzz.top/gtsdvngbkj.html

[U08] Py：展平二维列表
来源：http://hz.ivvv.top/gtudidngdv.html

[y for x in nested for y in x]
来源：http://hz.9152youxi.cn/gtkrczedsx.html

[U09] Py：字典取最大值的键
来源：http://hz.svipenyu.cn/gtznoamdmv.html

max(d, key=d.get)
来源：http://hz.feifeiyinyue.top/gtplweygyn.html

[U10] Py：按值排序字典
来源：http://hz.guowangkeji.top/gtttlrsiky.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhengqikj.top/gtayxonusw.html

[U11] Py：生成器表达式
来源：http://hz.tianlin.xyz/gtaftlryka.html

(x * 2 for x in arr)
来源：http://hz.yangfankeji.com/gtzahsvxlp.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.wangdashe.top/gtorjimnfl.html

Counter(arr).most_common(3)
来源：http://hz.zhixingplan.top/gtpxdnzpob.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtctuzrzai.html

deque(maxlen=10)
来源：http://hz.jlsjyb.cn/gtzwgcjcho.html

[U14] Py：分组收集到列表
来源：http://hz.tanke756.top/gtmqduufnj.html

defaultdict(list)
来源：http://hz.guowangkeji.top/gthyiqmlvl.html

[U15] Py：高精度计时
来源：http://hz.pycfn.com/gtbdlsebua.html

t = time.perf_counter()
来源：http://hz.ydjk.org.cn/gtlmjsxthu.html

[U16] Py：命令行参数解析
来源：http://hz.guowangkeji.top/gtfiigizem.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinghuilouyu.cn/gtbhfujkrv.html

[U17] Py：初始化日志
来源：http://hz.andypj.xyz/gtpgntebyp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhixingplan.top/gtugkoyxts.html

[U18] Py：预编译正则
来源：http://hz.tanke756.top/gtffamyhwr.html

pat = re.compile(r"\d+")
来源：http://hz.zhixingplan.top/gtkzgccqrd.html

[U19] Py：正则替换带回调
来源：http://hz.jiagoushi.top/gtwkmtcyni.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xylfe.cn/gtlbbvkwha.html

[U20] Py：缓存函数结果
来源：http://hz.haohaochexian.top/gtkikpujlc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tian-w.cn/gtmjnjbutx.html

[U21] Py：自定义上下文管理器
来源：http://hz.xziqi.cn/gtsgwrwbyz.html

@contextlib.contextmanager
来源：http://hz.hnqzz.top/gtzasedzma.html

[U22] Py：矩阵转置
来源：http://hz.hnxiangtu.top/gtpuprxbae.html

list(zip(*m))
来源：http://hz.jqgufenzy.top/gtstpvvgdb.html

[U23] Py：分块读取大文件
来源：http://hz.bjfxy.top/gtxgjugifl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zycfv.cn/gtbpyxwmxw.html

[U24] Py：路径操作
来源：http://hz.zhijiandao.cn/gtvscsrpgg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.quarkkingdee.top/gtwtvkffhw.html

[U25] Py：CSV 按字典读
来源：http://hz.yvedp.cn/gtvbdjfcpo.html

csv.DictReader(f)
来源：http://hz.cqqwz.cn/gtszgqvawr.html

[U26] Py：并发下载
来源：http://hz.havefunace.top/gtpglqkzds.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ywan-chungtsiang.top/gtdpymwstl.html

[U27] Py：异步 HTTP
来源：http://hz.jinqigufen.top/gtdzhnrhfl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jlsjyb.cn/gtvvgmcfmq.html

[U28] Py：类型别名
来源：http://hz.zhengqikj.top/gtnauetjmu.html

UserId = int
来源：http://hz.havefunace.top/gtgobdjzch.html

[U29] Py：属性校验
来源：http://hz.jlsjyb.cn/gtmhnjmful.html

@property 与 @x.setter 配合
来源：http://hz.feifeiyinyue.top/gtvztwexob.html

[U30] Py：数据类
来源：http://hz.hnqzz.top/gtzainezcq.html

@dataclass(slots=True)
来源：http://hz.9152youxi.cn/gtujzmrzdd.html

[U31] Py：单测
来源：http://hz.meibo888.top/gttmqyyesu.html

python -m pytest -q
来源：http://hz.ywan-chungtsiang.top/gtqcnmttls.html

[U32] Py：代码格式化
来源：http://hz.52xcode.cn/gtbeukhzgq.html

ruff format . && ruff check --fix .
来源：http://hz.yueranfly.top/gtopgjsasp.html

[U33] Py：打包发布
来源：http://hz.redwolf501.top/gtxmvhwhpu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cucudq.cn/gtdmxttvma.html

[U34] Py：判断编码
来源：http://hz.316326.xyz/gthqmtpbnp.html

chardet.detect(raw)
来源：http://hz.aibaodan.cn/gtztcxmpyi.html

[U35] Py：发送邮件
来源：http://hz.cashguo.top/gtvuidjiwp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nanxuanxn.top/gthuengies.html

[U36] Py：定时任务
来源：http://hz.gogol.net.cn/gtakihywwd.html

schedule.every(10).minutes.do(job)
来源：http://hz.tianlin.xyz/gttmcgkans.html

[U37] Py：读写 Excel
来源：http://hz.guannengcc.top/gtmojbllcv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tanke756.top/gtkjuliqau.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenzaomai.com/gtdpgwvlhl.html

Path(__file__).resolve().parent
来源：http://hz.cashguo.top/gtipcjttbx.html

[U39] Py：判断是否在交互环境
来源：http://hz.havefunace.top/gtydaeuhmz.html

sys.stdout.isatty()
来源：http://hz.wangshuangyany.cn/gtmqarxpwa.html

[U40] Py：打印到标准错误
来源：http://hz.yueranfly.top/gtlxwqpgcf.html

print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtrddskaqs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hywenlv.cn/gtlmfiqush.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenlongwang.top/gtpafbmugr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.guannengcc.top/gtwcvruspm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xuetiantiany.cn/gtuoxqckix.html

[U43] PHP：声明命名空间
来源：http://hz.daxiang520.top/gtsziscfwf.html

namespace App\Http;
来源：http://hz.kuanghao11.cn/gtanjweorx.html

[U44] PHP：开启严格类型
来源：http://hz.chenzaomai.com/gtbsfpyjws.html

declare(strict_types=1);
来源：http://hz.shangyingyoupin.top/gtxztrxgtm.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xuanzx.com/gtcgxkxjle.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtynhnutkg.html

[U46] PHP：可空类型
来源：http://hz.cucudq.cn/gtdhxqigfo.html

?string $name = null
来源：http://hz.dianchejie.cn/gtcsymgqty.html

[U47] PHP：联合类型
来源：http://hz.tianlin.xyz/gtsiycfgxl.html

int|string $id
来源：http://hz.yangfankeji.com/gtyjvelfel.html

[U48] PHP：纯枚举
来源：http://hz.ydzc1.top/gttyzwilwg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xingfuxueyuan.xyz/gtosqseahz.html

[U49] PHP：只读属性
来源：http://hz.chenjidiqi.icu/gtmpgdxsme.html

public readonly string $name
来源：http://hz.chenzaomai.com/gtxondtymj.html

[U50] PHP：构造器属性提升
来源：http://hz.redwolf501.top/gtjimvubhx.html

public function __construct(private int $id) {}
来源：http://hz.sysykeji.top/gtlxkluryp.html

[U51] PHP：数组解构
来源：http://hz.shangyingyoupin.top/gtftavsrjx.html

[$a, $b] = $arr;
来源：http://hz.xuanzx.com/gtmnmkflfl.html

[U52] PHP：箭头函数
来源：http://hz.zhixingplan.top/gteqxpybrv.html

$double = fn($x) => $x * 2;
来源：http://hz.tanke756.top/gtzurxvqkz.html

[U53] PHP：空合并运算符
来源：http://hz.hammf.cn/gtsksrjjvv.html

$v = $a ?? $b ?? "default";
来源：http://hz.nanxinkj.top/gthwdtpxto.html

[U54] PHP：空安全调用
来源：http://hz.hammf.cn/gtmbbaxlej.html

$obj?->method()
来源：http://hz.gogol.net.cn/gtdfqgjlgb.html

[U55] PHP：match 表达式
来源：http://hz.sufxvd.cn/gtmnupqthc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hnqzz.top/gtpxybxfzw.html

[U56] PHP：命名参数
来源：http://hz.zhoulong.xyz/gtripdkoih.html

f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtnwnzskod.html

[U57] PHP：字符串插值
来源：http://hz.cheryme.top/gtmjnjthts.html

"值: {$a}"
来源：http://hz.meibo888.top/gtjlzkrado.html

[U58] PHP：数组三件套
来源：http://hz.hammf.cn/gtikjwqwtv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.wangshuangyany.cn/gtmtpillmq.html

[U59] PHP：自定义排序
来源：http://hz.redwolf501.top/gtpafxzqzf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtpppdntao.html

[U60] PHP：JSON 编解码
来源：http://hz.smart0.xyz/gtsbqzuxqw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.daxiang520.top/gtxsnpyyjw.html

[U61] PHP：正则
来源：http://hz.tanke756.top/gtjjraandc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtmqjlgvyk.html

[U62] PHP：日期对象
来源：http://hz.shzxlz.cn/gtjcisucxd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.52xcode.cn/gtrnjnvcxg.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangtech.top/gtjgigycie.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yueranfly.top/gtljjgrevx.html

[U64] PHP：目录遍历
来源：http://hz.jinyuanbaomall.cn/gtymapcasn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xingfuxueyuan.xyz/gtdzubypfw.html

[U65] PHP：会话
来源：http://hz.guannengcc.top/gtllhjyakr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj20258888.top/gtiicsmnze.html

[U66] PHP：设置 Cookie
来源：http://hz.meibo888.top/gtlnuykgiz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.chenlongwang.top/gthmbdqfxd.html

[U67] PHP：处理文件上传
来源：http://hz.cdnleiting.top/gthssmqxwa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xingfuxueyuan.xyz/gtaxyzckrz.html

[U68] PHP：PDO 连接
来源：http://hz.pengpengdd.cyou/gtyaozocdz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhengqikj.top/gtzrnfkodc.html

[U69] PHP：PDO 预处理
来源：http://hz.nanxinkj.top/gtlfilpoap.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.wangshuangyany.cn/gthtbmmfko.html

[U70] PHP：PDO 事务
来源：http://hz.wangdashe.top/gtdbshraxx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.0kj1m.cn/gtukdmansq.html

[U71] PHP：抛出异常
来源：http://hz.zhijiandao.cn/gtnogkjltc.html

throw new RuntimeException("失败", 500);
来源：http://hz.jqgfzy.top/gtinwkyaqa.html

[U72] PHP：写错误日志
来源：http://hz.shuidangran.top/gtjvckpnvb.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shzxlz.cn/gtcajtuxji.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinyuanbaomall.cn/gtjmgrdhid.html

parse_ini_file("config.ini", true)
来源：http://hz.shzxlz.cn/gtcleqpddm.html

[U74] PHP：读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtrujnarsq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cdnleiting.top/gtdjdxedav.html

[U75] PHP：依赖注入
来源：http://hz.jinqigfzy.top/gtqjtcvdca.html

composer require psr/container
来源：http://hz.meibo888.top/gtmlfzqlsz.html

[U76] PHP：简单路由
来源：http://hz.cheryme.top/gtasutxbxe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gzhubu.top/gttszqotfh.html

[U77] PHP：模板渲染
来源：http://hz.gzhubu.top/gtzprvwhgh.html

composer require twig/twig
来源：http://hz.gotoacloud.top/gtenhoabxa.html

[U78] PHP：单元测试
来源：http://hz.andypj.xyz/gtyrvuxmoa.html

composer require --dev phpunit/phpunit
来源：http://hz.aibaodan.cn/gtxlgbxqtz.html

[U79] PHP：静态分析
来源：http://hz.gotoacloud.top/gtmrtxhefb.html

composer require --dev phpstan/phpstan
来源：http://hz.chenjidiqi.icu/gtgrjltqfb.html

[U80] PHP：代码规范修复
来源：http://hz.shanyushiyangtech.top/gtmiysjmsv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.aizwys.cn/gtoivpvcmk.html

[U81] JS：初始化项目
来源：http://hz.cashguo.top/gtavxpnrhh.html

npm init -y;  npm i express
来源：http://hz.shuidangran.top/gtbmemopky.html

[U82] JS：package.json 脚本
来源：http://hz.hnqzz.top/gtpairmnpx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gogol.net.cn/gteovhjmhr.html

[U83] JS：ES Module 导入导出
来源：http://hz.dianchejie.cn/gtigfatoxh.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.guannengcc.top/gtmiodannn.html

[U84] JS：CommonJS 写法
来源：http://hz.zhaomingkeji.xyz/gtmydlezdi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.nwbrower.top/gtmhjrcpph.html

[U85] JS：可选链
来源：http://hz.wangshuangyany.cn/gtmxtkbysy.html

a?.b?.c
来源：http://hz.ydjk.org.cn/gtldsrzwki.html

[U86] JS：空值合并
来源：http://hz.daria6918.cn/gtrstrdsrs.html

a ?? b
来源：http://hz.yvedp.cn/gtgcblzuqe.html

[U87] JS：解构默认值
来源：http://hz.jlsjyb.cn/gtbzukbtwd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhixingplan.top/gttoxyjlzg.html

[U88] JS：对象展开合并
来源：http://hz.pycfn.com/gtuewhsrva.html

{ ...a, ...b }
来源：http://hz.nwbrower.top/gtvyelmjdw.html

[U89] JS：数组去重
来源：http://hz.kuanghao11.cn/gtdaqbxfwj.html

[...new Set(arr)]
来源：http://hz.bjfxy.top/gtcdaneezy.html

[U90] JS：数字数组排序
来源：http://hz.yj202588.top/gtpouxqpji.html

[...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtpqdqxxvt.html

[U91] JS：对象键值遍历
来源：http://hz.jinghuilouyu.cn/gtgyfdftfb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ybcxt.top/gtgcczaqct.html

[U92] JS：深拷贝
来源：http://hz.sysykeji.top/gtztipjwou.html

structuredClone(obj)
来源：http://hz.cucudq.cn/gtfoswqsxt.html

[U93] JS：模板字符串
来源：http://hz.xuetiantiany.cn/gtovqdzwnu.html

`共 ${n} 条`
来源：http://hz.mhx1999.top/gtaxevyrmi.html

[U94] JS：箭头函数
来源：http://hz.smart0.xyz/gtlfszpmbo.html

const double = x => x * 2;
来源：http://hz.xylfe.cn/gttxzcvgsq.html

[U95] JS：Promise 包装
来源：http://hz.dianchejie.cn/gtpdxhkkxu.html

new Promise((resolve, reject) => {})
来源：http://hz.redwolf501.top/gtvlxkzogm.html

[U96] JS：async/await 与异常
来源：http://hz.316326.xyz/gtiatuacnk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtizelwacc.html

[U97] JS：并发请求
来源：http://hz.sxryk.cn/gtwprnxtss.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtthjkgpaj.html

[U98] JS：fetch 带 JSON
来源：http://hz.redwolf501.top/gttvmvrbqu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jinyuanbaomall.cn/gtfytsxikh.html

[U99] JS：事件监听
来源：http://hz.zdqjudy.top/gtkbcijpwu.html

el.addEventListener("click", e => {})
来源：http://hz.yueranfly.top/gtjodcuaeb.html

[U100] JS：DOM 查询
来源：http://hz.cqqwz.cn/gtehbnitfr.html

document.querySelector(".item")
来源：http://hz.zycfv.cn/gtlmplhysk.html

[U101] JS：classList 操作
来源：http://hz.chenzaomai.com/gtkkyxeytb.html

el.classList.toggle("active")
来源：http://hz.sufxvd.cn/gtqozdncne.html

[U102] JS：本地存储
来源：http://hz.316326.xyz/gtjyucalmi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.0kj1m.cn/gturwxdtrr.html

[U103] JS：定时器
来源：http://hz.tianlin.xyz/gtgzdzypmm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.tanke756.top/gtzbzqnaqa.html

[U104] JS：防抖
来源：http://hz.tianlin.xyz/gtnievliig.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtshxbkkdz.html

[U105] JS：节流
来源：http://hz.chenjidiqi.icu/gtsashjwmd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.quarkkingdee.top/gtmmqscfjy.html

[U106] JS：日期格式化
来源：http://hz.sweek.top/gtwiwlbuln.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jianghu66.top/gtiwgufvzf.html

[U107] JS：数字千分位
来源：http://hz.chenzaomai.com/gtgtheopvu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cdnleiting.top/gtcringzfi.html

[U108] JS：随机整数
来源：http://hz.fengsongda.top/gtxlqypnel.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guannengcc.top/gtyijksyyg.html

[U109] JS：数组分组
来源：http://hz.316326.xyz/gtltbnieuq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtpwzxjhkx.html

[U110] JS：数组分块
来源：http://hz.birdmap.top/gtnfaogcbd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhijiandao.cn/gtppomlawn.html

[U111] JS：对象转 Map
来源：http://hz.jlsjyb.cn/gtlujadclo.html

new Map(Object.entries(obj))
来源：http://hz.ehwqpu.com/gtgovddrka.html

[U112] JS：字符串补位
来源：http://hz.mhx1999.top/gtcavlnpdx.html

"7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gteszfsazb.html

[U113] JS：正则替换全部
来源：http://hz.yueranfly.top/gtqkpbakuc.html

s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtpycmmocz.html

[U114] JS：JSON 深比较
来源：http://hz.daxiang520.top/gtziqowgrl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtqmnlsefi.html

[U115] JS：生成 UUID
来源：http://hz.52xcode.cn/gthavlytmy.html

crypto.randomUUID()
来源：http://hz.ydzc1.top/gtcinaijfw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ivvv.top/gtpsmtadzb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zdqjudy.top/gtoukncwmf.html

[U117] JS：单元测试
来源：http://hz.ydjk.org.cn/gtdmkpfkny.html

npm i -D vitest;  npx vitest
来源：http://hz.yanxiufei.cn/gtyyemqbux.html

[U118] JS：开发服务器
来源：http://hz.pycfn.com/gtextbuyuy.html

npm i -D vite;  npx vite
来源：http://hz.snrcjt.cn/gtxokvkwdd.html

[U119] JS：生产构建
来源：http://hz.daria6918.cn/gtzysixehv.html

npx vite build
来源：http://hz.cdnleiting.top/gtdgsakzjz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cheryme.top/gtidzelfzn.html

import.meta.env.VITE_API_URL
来源：http://hz.xuanzx.com/gtxmpanzom.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxqgslpfy.html

统计汇总
来源：http://hz.zhijiandao.cn/gtcgpbylvv.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtunzgoqgy.html

按语言统计（条）：
来源：http://hz.snrcjt.cn/gtfgigxszi.html

Python ......... 252
来源：http://hz.xinyue.icu/gtkalhtlha.html

PHP ............ 252
来源：http://hz.sweek.top/gtbjbmbjkr.html

JavaScript ..... 252
来源：http://hz.xuanzx.com/gtsqzxynrx.html

TypeScript ..... 212
来源：http://hz.gogol.net.cn/gtzbmcxour.html

Java ........... 212
来源：http://hz.jyoumei.cn/gtaenhcudd.html

Go ............. 212
来源：http://hz.gotoacloud.top/gtvaudwrhe.html

Ruby ........... 212
来源：http://hz.ehwqpu.com/gtrjqfkksw.html

C# ............. 212
来源：http://hz.ehwqpu.com/gtplonjxhw.html

C .............. 30
来源：http://hz.0kj1m.cn/gtzpwfzhcj.html

C++ ............ 30
来源：http://hz.jqgfzy.top/gtbdyozhrw.html

SQL ............ 90
来源：http://hz.gotoacloud.top/gtqfkpkfdn.html

Bash ........... 80
来源：http://hz.nanxuanxn.top/gtqwmtoeol.html

Kotlin ......... 15
来源：http://hz.zhongyouzk.top/gtmyynwejm.html

Swift .......... 15
来源：http://hz.quarkkingdee.top/gtwwumruoh.html

Lua ............ 10
来源：http://hz.yj202588.top/gtecaeutvc.html

Perl ........... 10
来源：http://hz.hfpthk.cn/gtaifpfnoj.html

Scala .......... 10
来源：http://hz.redwolf501.top/gtojrqaqkm.html

------------------------------------
来源：http://hz.xinyue.icu/gtxwfleoix.html

合计 ........... 2106 条
来源：http://hz.hywenlv.cn/gtenvtbcoc.html

按章节统计：
来源：http://hz.0kj1m.cn/gtyrvwfuix.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cashguo.top/gtdoyxxawn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtpuwsgchf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gthyhgoofs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.andypj.xyz/gttzhzqkbx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shangyingyoupin.top/gtjnwrwetz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xziqi.cn/gtrphjebzn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtlgwurzgr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangdashe.top/gtqqgigsff.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtoeecxiko.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shangyingyoupin.top/gtibjqckgs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtxmmyrkyy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtyivmypyd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtivfpylfh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yuanzhike.top/gtunsguifm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.gotoacloud.top/gtlrznxmvg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtfnhpolpg.html

Q SQL 专题                              90
来源：http://hz.hfpthk.cn/gtsvzjhnxo.html

R Bash 专题                             80
来源：http://hz.chenlongwang.top/gtnbsznpgf.html

S C / C++ 专题                          60
来源：http://hz.andypj.xyz/gtzglkxalx.html

T 其他语言补充                          60
来源：http://hz.hysaishi.cn/gtziggmang.html

U 高频实用片段                         120
来源：http://hz.gzhubu.top/gttxpvurvm.html

------------------------------------
来源：http://hz.9152youxi.cn/gtnselkwux.html

合计                                  2106 条
来源：http://hz.yuanzhike.top/gthhscjsio.html

--------------------------------------------------------------------------------
来源：http://hz.fengsongda.top/gtfdcnvwgb.html


<!-- 参考信息 -->