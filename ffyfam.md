代发 wailian999

[U17] Py：初始化日志
来源：http://hz.sweek.top/gtyquwtcfs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.iojbl.cn/gtdocjtpua.html

[U18] Py：预编译正则
来源：http://hz.zhongyouzk.top/gtzyxrtysk.html

pat = re.compile(r"\d+")
来源：http://hz.xuanzx.com/gtjdxmvuse.html

[U19] Py：正则替换带回调
来源：http://hz.sweek.top/gtszmuwacm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.pengpengdd.cyou/gtppkxreop.html

[U20] Py：缓存函数结果
来源：http://hz.meibo888.top/gtxpsiarnj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shanyushiyangkeji.top/gtcespgyie.html

[U21] Py：自定义上下文管理器
来源：http://hz.nanxuanxn.top/gtzbdblsbs.html

@contextlib.contextmanager
来源：http://hz.jianghu66.top/gtrhywaelj.html

[U22] Py：矩阵转置
来源：http://hz.shuidangran.top/gttedpcbsn.html

list(zip(*m))
来源：http://hz.shzxlz.cn/gtheqslovq.html

[U23] Py：分块读取大文件
来源：http://hz.yuxming.cn/gteourjtqh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sxryk.cn/gtbjjhjqdz.html

[U24] Py：路径操作
来源：http://hz.hnxiangtu.top/gtckfooyso.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hysaishi.cn/gtziziychk.html

[U25] Py：CSV 按字典读
来源：http://hz.yvedp.cn/gtgshuazbt.html

csv.DictReader(f)
来源：http://hz.yongpay.top/gtawouyxve.html

[U26] Py：并发下载
来源：http://hz.wangshuangyany.cn/gtnypfypxi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ywan-chungtsiang.top/gteuhvvpqy.html

[U27] Py：异步 HTTP
来源：http://hz.cucudq.cn/gtxkhhadqo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dashuyun.cn/gtvtfazwwz.html

[U28] Py：类型别名
来源：http://hz.hfpthk.cn/gtxjjmcqmn.html

UserId = int
来源：http://hz.cdnleiting.top/gtjbfjioiy.html

[U29] Py：属性校验
来源：http://hz.nanxuanxn.top/gttdhjjmnh.html

@property 与 @x.setter 配合
来源：http://hz.sweek.top/gtdxwtqmza.html

[U30] Py：数据类
来源：http://hz.aibaodan.cn/gtswwgxqto.html

@dataclass(slots=True)
来源：http://hz.yongpay.top/gtlnriarlw.html

[U31] Py：单测
来源：http://hz.gotoacloud.top/gtnppsmdzt.html

python -m pytest -q
来源：http://hz.xuetiantiany.cn/gtrymsdtbj.html

[U32] Py：代码格式化
来源：http://hz.jlsjyb.cn/gtqysuuhca.html

ruff format . && ruff check --fix .
来源：http://hz.0kj1m.cn/gtqaswrkfr.html

[U33] Py：打包发布
来源：http://hz.zhengqikj.top/gtfotytgmc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xingfuxueyuan.xyz/gtaskyucze.html

[U34] Py：判断编码
来源：http://hz.zdqjudy.top/gtdrebsmso.html

chardet.detect(raw)
来源：http://hz.chenlongwang.top/gtnbdxmyjs.html

[U35] Py：发送邮件
来源：http://hz.pycfn.com/gttzhlgnnc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.pycfn.com/gtjrndnlnb.html

[U36] Py：定时任务
来源：http://hz.aibaodan.cn/gtculbamzq.html

schedule.every(10).minutes.do(job)
来源：http://hz.andypj.xyz/gtfhahptaj.html

[U37] Py：读写 Excel
来源：http://hz.yj20258.top/gthodxvazv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sufxvd.cn/gtvrcyevxu.html

[U38] Py：获取脚本所在目录
来源：http://hz.jiagoushi.top/gtxasfznsh.html

Path(__file__).resolve().parent
来源：http://hz.andypj.xyz/gtscwpyukf.html

[U39] Py：判断是否在交互环境
来源：http://hz.cucudq.cn/gthbqhvaoe.html

sys.stdout.isatty()
来源：http://hz.quarkkingdee.top/gtavawnbjs.html

[U40] Py：打印到标准错误
来源：http://hz.hnxiangtu.top/gtesyqvtuz.html

print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtieocgxmj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinqigfzy.top/gtgdybhmlv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinyuanbaomall.cn/gtdoutfdnv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.52xcode.cn/gtztywnwpk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.havefunace.top/gtpwnhwfyg.html

[U43] PHP：声明命名空间
来源：http://hz.haohaochexian.top/gtkwxvclsq.html

namespace App\Http;
来源：http://hz.fzhhl.top/gtosbolbxw.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtkvbhrwfy.html

declare(strict_types=1);
来源：http://hz.zhengqikj.top/gtmgkzvaff.html

[U45] PHP：类型声明与返回类型
来源：http://hz.mhx1999.top/gtwlkxdmib.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtztmdbkms.html

[U46] PHP：可空类型
来源：http://hz.pycfn.com/gtnzfhdhar.html

?string $name = null
来源：http://hz.wangshuangyany.cn/gtrrnzqaux.html

[U47] PHP：联合类型
来源：http://hz.shanyushiyangkeji.top/gtpbxrowdn.html

int|string $id
来源：http://hz.dianchejie.cn/gtsgyjkojt.html

[U48] PHP：纯枚举
来源：http://hz.hongshengwenyu.top/gtmozmoiuj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhixingplan.top/gtthgwzhaa.html

[U49] PHP：只读属性
来源：http://hz.xuanzx.com/gtqmlhnguw.html

public readonly string $name
来源：http://hz.gogol.net.cn/gtzemeposk.html

[U50] PHP：构造器属性提升
来源：http://hz.yvedp.cn/gthuqaekxc.html

public function __construct(private int $id) {}
来源：http://hz.jianghu66.top/gtdtywytbf.html

[U51] PHP：数组解构
来源：http://hz.zhixingplan.top/gthzihpugk.html

[$a, $b] = $arr;
来源：http://hz.kuanghao11.cn/gtvcviydlj.html

[U52] PHP：箭头函数
来源：http://hz.jinghuilouyu.cn/gtcpyovumg.html

$double = fn($x) => $x * 2;
来源：http://hz.sweek.top/gtbmyobkzf.html

[U53] PHP：空合并运算符
来源：http://hz.dashuyun.cn/gthqrqapqg.html

$v = $a ?? $b ?? "default";
来源：http://hz.gotoacloud.top/gtyduwbmbn.html

[U54] PHP：空安全调用
来源：http://hz.yanxiufei.cn/gtkwyoopve.html

$obj?->method()
来源：http://hz.yvedp.cn/gtnltourfj.html

[U55] PHP：match 表达式
来源：http://hz.ywan-chungtsiang.top/gtpkvzprbv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.wangdashe.top/gtzrdzrxhn.html

[U56] PHP：命名参数
来源：http://hz.yongpay.top/gtuldlelaf.html

f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtwxburkmh.html

[U57] PHP：字符串插值
来源：http://hz.jlsjyb.cn/gtutjvyqba.html

"值: {$a}"
来源：http://hz.jlsjyb.cn/gtoqxhokfg.html

[U58] PHP：数组三件套
来源：http://hz.dashuyun.cn/gtsylcdczd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ivvv.top/gtphlzncza.html

[U59] PHP：自定义排序
来源：http://hz.yj20258.top/gtpdjjjmme.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtesdpfnqy.html

[U60] PHP：JSON 编解码
来源：http://hz.zhiwuduotai.top/gtmfficypv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.andypj.xyz/gtgisuwetp.html

[U61] PHP：正则
来源：http://hz.hongshengwenyu.top/gtzvoxmizc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gtjkemcsdp.html

[U62] PHP：日期对象
来源：http://hz.hongshengwenyu.top/gtszljnkvg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.feifeiyinyue.top/gtlmamfklm.html

[U63] PHP：文件读写
来源：http://hz.wangdashe.top/gttpsephan.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shzxlz.cn/gtgrccsvzc.html

[U64] PHP：目录遍历
来源：http://hz.sysykeji.top/gtdhkgicwp.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnqzz.top/gthhibckuw.html

[U65] PHP：会话
来源：http://hz.vqdsnc.cn/gtcmmjhpvy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hysaishi.cn/gtomzaivlj.html

[U66] PHP：设置 Cookie
来源：http://hz.daxiang520.top/gtpqfihbvv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydzc1.top/gtdcumaugw.html

[U67] PHP：处理文件上传
来源：http://hz.fzhhl.top/gtbunltzuz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hammf.cn/gtjewouiqo.html

[U68] PHP：PDO 连接
来源：http://hz.316326.xyz/gtuovcovqq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.dashuyun.cn/gtstlxeobb.html

[U69] PHP：PDO 预处理
来源：http://hz.shuidangran.top/gtloswdpxf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.quarkkingdee.top/gtafsvisqu.html

[U70] PHP：PDO 事务
来源：http://hz.c1oappe.top/gtbjyscumq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.daria6918.cn/gtzedsijrp.html

[U71] PHP：抛出异常
来源：http://hz.fzhhl.top/gteldfxuor.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhiwuduotai.top/gtiatcpqai.html

[U72] PHP：写错误日志
来源：http://hz.cheryme.top/gtthfxwtsj.html

error_log("失败: " . $e->getMessage());
来源：http://hz.redwolf501.top/gtglfcakmc.html

[U73] PHP：读取 ini 配置
来源：http://hz.sysykeji.top/gtywzjgdhu.html

parse_ini_file("config.ini", true)
来源：http://hz.shanyushiyangtech.top/gtpbdrprsl.html

[U74] PHP：读取环境变量
来源：http://hz.xuanzx.com/gtjfpzfjwv.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sxryk.cn/gtxraqytgl.html

[U75] PHP：依赖注入
来源：http://hz.smart0.xyz/gtibzpqmfa.html

composer require psr/container
来源：http://hz.yuxming.cn/gtjsaixqjc.html

[U76] PHP：简单路由
来源：http://hz.ywan-chungtsiang.top/gtdtnzzwzw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.9152youxi.cn/gtzuxdpcwo.html

[U77] PHP：模板渲染
来源：http://hz.hfpthk.cn/gtphuoqanc.html

composer require twig/twig
来源：http://hz.jqgufenzy.top/gtfjjcsbfl.html

[U78] PHP：单元测试
来源：http://hz.zdqjudy.top/gtaszwjctm.html

composer require --dev phpunit/phpunit
来源：http://hz.haohaochexian.top/gtgqvasjnn.html

[U79] PHP：静态分析
来源：http://hz.nwbrower.top/gtlwixijvp.html

composer require --dev phpstan/phpstan
来源：http://hz.quarkkingdee.top/gtqzawqgqa.html

[U80] PHP：代码规范修复
来源：http://hz.c1oappe.top/gtnybgwfcx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cashguo.top/gthqvbeyls.html

[U81] JS：初始化项目
来源：http://hz.guannengcc.top/gtvuwycpuo.html

npm init -y;  npm i express
来源：http://hz.mhx1999.top/gtnkohwqnw.html

[U82] JS：package.json 脚本
来源：http://hz.dianchejie.cn/gtylzfgrcl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinqigufen.top/gtzxnmhxks.html

[U83] JS：ES Module 导入导出
来源：http://hz.316326.xyz/gtiwngkiil.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.tianlin.xyz/gtjnslkdtu.html

[U84] JS：CommonJS 写法
来源：http://hz.gzhubu.top/gtorjscebx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zdqjudy.top/gtshymzern.html

[U85] JS：可选链
来源：http://hz.hnxiangtu.top/gtysmxxnlh.html

a?.b?.c
来源：http://hz.shanyushiyangkeji.top/gtjtsojmsj.html

[U86] JS：空值合并
来源：http://hz.sweek.top/gtbhzxxqpg.html

a ?? b
来源：http://hz.gogol.net.cn/gtgfzccont.html

[U87] JS：解构默认值
来源：http://hz.ybcxt.top/gtxdlqanya.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tanke756.top/gtrdgqoclo.html

[U88] JS：对象展开合并
来源：http://hz.xuanzx.com/gtepjbemyk.html

{ ...a, ...b }
来源：http://hz.tianlin.xyz/gtuimbswtl.html

[U89] JS：数组去重
来源：http://hz.xuetiantiany.cn/gtqrgwgozj.html

[...new Set(arr)]
来源：http://hz.guannengcc.top/gtfpslihxb.html

[U90] JS：数字数组排序
来源：http://hz.vqdsnc.cn/gtdxpfyilk.html

[...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gtnnwxungz.html

[U91] JS：对象键值遍历
来源：http://hz.daria6918.cn/gtgaozjcdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jqgfzy.top/gtsyplgkeh.html

[U92] JS：深拷贝
来源：http://hz.sxryk.cn/gtalgdagqp.html

structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtiznmnofm.html

[U93] JS：模板字符串
来源：http://hz.cqqwz.cn/gtlipmiehk.html

`共 ${n} 条`
来源：http://hz.xingfuxueyuan.xyz/gtcjznlxie.html

[U94] JS：箭头函数
来源：http://hz.wangdashe.top/gtprgjvvci.html

const double = x => x * 2;
来源：http://hz.shzxlz.cn/gtvcabnwml.html

[U95] JS：Promise 包装
来源：http://hz.tian-w.cn/gtcsyjezan.html

new Promise((resolve, reject) => {})
来源：http://hz.daxiang520.top/gtblrrvarp.html

[U96] JS：async/await 与异常
来源：http://hz.hnxiangtu.top/gtchvvllyp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtdhagamte.html

[U97] JS：并发请求
来源：http://hz.aizwys.cn/gtdcrnypkd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtnyqjgbhc.html

[U98] JS：fetch 带 JSON
来源：http://hz.hfpthk.cn/gtivqyncmm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zdqjudy.top/gtdjsdmimq.html

[U99] JS：事件监听
来源：http://hz.guannengcc.top/gtnakrtmne.html

el.addEventListener("click", e => {})
来源：http://hz.cqqwz.cn/gtrhtafxno.html

[U100] JS：DOM 查询
来源：http://hz.jianghu66.top/gtjqedpebo.html

document.querySelector(".item")
来源：http://hz.shanyushiyangtech.top/gtfzgcqybj.html

[U101] JS：classList 操作
来源：http://hz.hammf.cn/gtpfpyxdvz.html

el.classList.toggle("active")
来源：http://hz.jinqigufen.top/gtilmflnzp.html

[U102] JS：本地存储
来源：http://hz.hysaishi.cn/gtwkumrgtn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinqigufen.top/gtymlxzdnx.html

[U103] JS：定时器
来源：http://hz.cheryme.top/gtxfdzonew.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.snrcjt.cn/gthpplocgx.html

[U104] JS：防抖
来源：http://hz.shanyushiyangtech.top/gtpcpynebq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtlhgxuigx.html

[U105] JS：节流
来源：http://hz.xuetiantiany.cn/gtvvewdfje.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenzaomai.com/gttygcxanr.html

[U106] JS：日期格式化
来源：http://hz.feifeiyinyue.top/gtemibqcru.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ywan-chungtsiang.top/gtkjyollhv.html

[U107] JS：数字千分位
来源：http://hz.jinqigufen.top/gtjwyfbqkz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.sxryk.cn/gtsjfnxjlu.html

[U108] JS：随机整数
来源：http://hz.hammf.cn/gtbdgwdmfg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hongshengwenyu.top/gthonpvnqk.html

[U109] JS：数组分组
来源：http://hz.tian-w.cn/gtrwezgdgm.html

Object.groupBy(arr, x => x.type)
来源：http://hz.guannengcc.top/gtaxzzuwdb.html

[U110] JS：数组分块
来源：http://hz.xuetiantiany.cn/gtehjlhnqc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.smart0.xyz/gtrgccgyqt.html

[U111] JS：对象转 Map
来源：http://hz.hywenlv.cn/gtnouhgyfa.html

new Map(Object.entries(obj))
来源：http://hz.hnxiangtu.top/gtqeospftk.html

[U112] JS：字符串补位
来源：http://hz.shzxlz.cn/gtsluddwvf.html

"7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtdwpluhqy.html

[U113] JS：正则替换全部
来源：http://hz.yj202588.top/gtkkqhqodd.html

s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtvcyglrlh.html

[U114] JS：JSON 深比较
来源：http://hz.hysaishi.cn/gtahognrvd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtmpnvmyzd.html

[U115] JS：生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtswsyjsdk.html

crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtzwruzpza.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.havefunace.top/gtujmhhfkr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dianchejie.cn/gteexijxoz.html

[U117] JS：单元测试
来源：http://hz.yongpay.top/gtgiixjabl.html

npm i -D vitest;  npx vitest
来源：http://hz.ydjk.org.cn/gtsagslsyr.html

[U118] JS：开发服务器
来源：http://hz.zycfv.cn/gtsmupzapj.html

npm i -D vite;  npx vite
来源：http://hz.zhoulong.xyz/gtyqkahljd.html

[U119] JS：生产构建
来源：http://hz.c1oappe.top/gtogqkomlx.html

npx vite build
来源：http://hz.0kj1m.cn/gtnbmqrbla.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yongpay.top/gtlrvvibak.html

import.meta.env.VITE_API_URL
来源：http://hz.meibo888.top/gtuldbiore.html

================================================================================
来源：http://hz.pycfn.com/gtqfuaimll.html

统计汇总
来源：http://hz.zhengqikj.top/gtqztrajxm.html

================================================================================
来源：http://hz.yj20258888.top/gtiuescfgv.html

按语言统计（条）：
来源：http://hz.cucudq.cn/gtaatnhpid.html

Python ......... 252
来源：http://hz.wangshuangyany.cn/gttgjtspyf.html

PHP ............ 252
来源：http://hz.zhijiandao.cn/gtloryoafh.html

JavaScript ..... 252
来源：http://hz.daria6918.cn/gtbadhqwar.html

TypeScript ..... 212
来源：http://hz.wangshuangyany.cn/gtolguwnpc.html

Java ........... 212
来源：http://hz.haohaochexian.top/gtjzqyqxcg.html

Go ............. 212
来源：http://hz.hongshengwenyu.top/gtddhahazv.html

Ruby ........... 212
来源：http://hz.wangshuangyany.cn/gtdyskikyi.html

C# ............. 212
来源：http://hz.jyoumei.cn/gtihbbcwue.html

C .............. 30
来源：http://hz.chenzaomai.com/gtlpljhams.html

C++ ............ 30
来源：http://hz.fzhhl.top/gtkvjtksmz.html

SQL ............ 90
来源：http://hz.chenzaomai.com/gtbovrpxli.html

Bash ........... 80
来源：http://hz.cucudq.cn/gtokeuujvg.html

Kotlin ......... 15
来源：http://hz.wangshuangyany.cn/gtpjiuajhu.html

Swift .......... 15
来源：http://hz.hysaishi.cn/gtkxjdsqui.html

Lua ............ 10
来源：http://hz.9152youxi.cn/gtiwzaghji.html

Perl ........... 10
来源：http://hz.zhongyouzk.top/gtcxpjyqof.html

Scala .......... 10
来源：http://hz.haohaochexian.top/gtmmzliqqh.html

------------------------------------
来源：http://hz.jqgufenzy.top/gtrbajwfcf.html

合计 ........... 2106 条
来源：http://hz.shanyushiyangkeji.top/gtpcfryzyi.html

按章节统计：
来源：http://hz.c1oappe.top/gtosrbwuxp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gtncllpgcs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258.top/gtgybmwqjg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ppjwa.cn/gtdwfesxca.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.0kj1m.cn/gtccuizwim.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shanyushiyangkeji.top/gtympkieab.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gogol.net.cn/gtwkupoggo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.snrcjt.cn/gtpsacdjhs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtoexgcyzo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtoksezkzb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtcsqitvgg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtfuwtgwfu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtciblvicr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gteidngwkk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtvdomsdcc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xinyue.icu/gthxldzzst.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtoqgroslf.html

Q SQL 专题                              90
来源：http://hz.andypj.xyz/gtybsmhvqk.html

R Bash 专题                             80
来源：http://hz.bjfxy.top/gtwglqrtii.html

S C / C++ 专题                          60
来源：http://hz.xuanzx.com/gtfpdqgwsj.html

T 其他语言补充                          60
来源：http://hz.yuxming.cn/gtulleckql.html

U 高频实用片段                         120
来源：http://hz.hongshengwenyu.top/gtknujapuz.html

------------------------------------
来源：http://hz.birdmap.top/gtmmgmqnts.html

合计                                  2106 条
来源：http://hz.yj20258888.top/gtjtidigpv.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtoyzvuiat.html

使用提醒
来源：http://hz.xylfe.cn/gtthdvmhea.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtoydbnarc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nwbrower.top/gtgwwsoqxe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yj20258888.top/gtxwfubpom.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jqgufenzy.top/gtncvnmkhk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gtwkdxcuvh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shanyushiyangkeji.top/gtehqdunvg.html

—— 文件结束 ——
来源：http://hz.mhx1999.top/gtixjyrjbx.html

================================================================================
来源：http://hz.yj202588.top/gtahiqzmnl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenlongwang.top/gtnewhtaqh.html

Common Programming Examples Cheat Book
来源：http://hz.quarkkingdee.top/gtjmsubxqt.html

================================================================================
来源：http://hz.316326.xyz/gtjglqjqbl.html

【收录内容】
来源：http://hz.dashuyun.cn/gtqyaoswux.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhiwuduotai.top/gtgnebiwby.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.chenjidiqi.icu/gtvupjkodz.html

SQL · Bash · C · C++
来源：http://hz.xingfuxueyuan.xyz/gtgyfjpwzx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.shangyingyoupin.top/gtjidxfruk.html

【使用说明】
来源：http://hz.cucudq.cn/gtkpmnvexr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yonumen.top/gtsxtmqyvl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shzxlz.cn/gtkaylqscf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.nanxinkj.top/gthlnesfth.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sysykeji.top/gtkzlsjqje.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yuanzhike.top/gtyihxtarq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jinqigfzy.top/gtotwnfaid.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hywenlv.cn/gtjgjjecmb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ywan-chungtsiang.top/gtqubwiakf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.9152youxi.cn/gtgwzvgtru.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.dashuyun.cn/gtmpxlprkd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.dianchejie.cn/gthdntqlgm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.guowangkeji.top/gtjombcmzr.html

【文件统计】
来源：http://hz.jinqigufen.top/gtkaserraf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ppjwa.cn/gtcmnbfbyh.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtdkgewyfe.html

目  录
来源：http://hz.yuxming.cn/gtjqcveirr.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtumljraqv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhijiandao.cn/gtuqtkddrq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.sysykeji.top/gtzcpbdlgk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.wangshuangyany.cn/gtkgzaxijp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shzxlz.cn/gtxjyiiudr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xuanzx.com/gtubrqviyc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.9152youxi.cn/gthsvxtkje.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.kuanghao11.cn/gtaixxdqvp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xuanzx.com/gtsbpyuyqx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jiagoushi.top/gtlyxuupcc.html


<!-- 参考信息 -->