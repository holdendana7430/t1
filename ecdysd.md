代发 wailian999

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtownirxhb.html

[R38] 管道串联
来源：http://hz.yonumen.top/gterflthfz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuanzx.com/gtrgzhwqhw.html

[R39] 重定向标准输出与错误
来源：http://hz.zhixingplan.top/gtcsiswgkv.html

cmd > out.log 2>&1
来源：http://hz.gogol.net.cn/gtprmlrczb.html

[R40] 追加写日志
来源：http://hz.jqgufenzy.top/gtujvhujvy.html

echo "log" >> out.log
来源：http://hz.sxryk.cn/gtgxsjdjtz.html

[R41] 丢弃输出
来源：http://hz.daxiang520.top/gtpnyiugpc.html

cmd >/dev/null 2>&1
来源：http://hz.yonumen.top/gtsfntajuo.html

[R42] 输入重定向
来源：http://hz.jiagoushi.top/gtegcpzfgh.html

wc -l < a.txt
来源：http://hz.jlsjyb.cn/gtfeskbrsk.html

[R43] 按名字查找文件
来源：http://hz.ppjwa.cn/gtahesoxlw.html

find . -name "*.log" -type f
来源：http://hz.wangshuangyany.cn/gtxgszefux.html

[R44] 按修改时间查找
来源：http://hz.zhaomingkeji.xyz/gttmywbnen.html

find . -mtime -7 -type f
来源：http://hz.yj202588.top/gtuxlkfhzd.html

[R45] 批量删除
来源：http://hz.nanxuanxn.top/gtpzbwglet.html

find . -name "*.tmp" -delete
来源：http://hz.jinghuilouyu.cn/gtlzbjseub.html

[R46] 递归替换文件内容
来源：http://hz.xingfuxueyuan.xyz/gtsxvizyxa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aibaodan.cn/gtqftvklry.html

[R47] sed 单行替换
来源：http://hz.redwolf501.top/gtolsaqiev.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuetiantiany.cn/gtyslfmxub.html

[R48] awk 取指定列
来源：http://hz.zhaomingkeji.xyz/gtirbupzqf.html

awk '{print $1, $3}' a.txt
来源：http://hz.guannengcc.top/gtwxdwugrc.html

[R49] awk 带条件
来源：http://hz.shanyushiyangtech.top/gtuvezyyhr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtngtdhzqh.html

[R50] awk 求和
来源：http://hz.zhiwuduotai.top/gtrlwlscok.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yueranfly.top/gtjuiqxcah.html

[R51] 排序去重取前几
来源：http://hz.daxiang520.top/gtbiyhcndl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhijiandao.cn/gtynybadpa.html

[R52] 统计行数
来源：http://hz.dashuyun.cn/gthqkzyyzy.html

wc -l a.txt
来源：http://hz.birdmap.top/gtrlzfxpji.html

[R53] 查看文件头与实时尾
来源：http://hz.hnqzz.top/gtrydfojil.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gogol.net.cn/gtgbqtubgf.html

[R54] 比较两个文件
来源：http://hz.yvedp.cn/gtgysbmdjm.html

diff a.txt b.txt
来源：http://hz.hnqzz.top/gthvpgorwr.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gtakrnnjbn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ybcxt.top/gttntcgoon.html

[R56] 远程拷贝
来源：http://hz.fengsongda.top/gtfvrdzrle.html

scp file user@host:/path/
来源：http://hz.chenlongwang.top/gtoaxfgxfk.html

[R57] 远程执行命令
来源：http://hz.shzxlz.cn/gtqbehughj.html

ssh user@host 'uptime'
来源：http://hz.gaohongyu789.top/gtwwemtosp.html

[R58] 下载文件
来源：http://hz.cheryme.top/gtporogirz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtxfixysox.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtnrjjmbkm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gtkfldosmg.html

[R60] 只看 HTTP 状态码
来源：http://hz.fzhhl.top/gtckmxlfhs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shuidangran.top/gtkjqejqip.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gtknlqkcqs.html

df -h;  du -sh *
来源：http://hz.tian-w.cn/gtzlbymhvq.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gtifurewux.html

du -ah . | sort -rh | head -10
来源：http://hz.xziqi.cn/gtzdqtjrmx.html

[R63] 内存与进程
来源：http://hz.0kj1m.cn/gtjdpjlils.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gtbspkyhuj.html

[R64] 结束进程
来源：http://hz.fengsongda.top/gtqelydatn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj202588.top/gtnqkagxyt.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtbpgxjlwm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jiagoushi.top/gtgqdhvlxi.html

[R66] 定时任务
来源：http://hz.daxiang520.top/gtgqbarvfr.html

crontab -e;  crontab -l
来源：http://hz.52xcode.cn/gtmzgclfuc.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gthgesryfs.html

openssl rand -hex 16
来源：http://hz.jyoumei.cn/gtkxtateha.html

[R68] 计算文件校验值
来源：http://hz.jiagoushi.top/gtobsxbyqp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ppjwa.cn/gtowdlufxs.html

[R69] 生成随机密码
来源：http://hz.jinqigfzy.top/gtxhsebikh.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtwgtzihkw.html

[R70] 时间戳与互转
来源：http://hz.hnxiangtu.top/gtxunycsmj.html

date +%s;  date -d @1700000000
来源：http://hz.zhijiandao.cn/gtwbfzstgj.html

[R71] 日期格式化
来源：http://hz.316326.xyz/gtsssmexhj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tanke756.top/gtrnqnacjc.html

[R72] 等待端口就绪
来源：http://hz.jinghuilouyu.cn/gtziojyubz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hnqzz.top/gtwfquvbnb.html

[R73] 分割大日志
来源：http://hz.yonumen.top/gtkplhpkqt.html

split -l 1000 big.log part_
来源：http://hz.ydjk.org.cn/gtvpyunfpy.html

[R74] 批量重命名
来源：http://hz.zhongyouzk.top/gtghkyuomr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhaomingkeji.xyz/gtpgzzxzwk.html

[R75] 导出环境变量
来源：http://hz.vqdsnc.cn/gtqwxnnnwx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gttzywwtbf.html

[R76] 使用临时文件
来源：http://hz.chenzaomai.com/gtpgwyepgb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtyltmcjjl.html

[R77] 读取用户输入
来源：http://hz.fzhhl.top/gtdxjgfnru.html

read -rp "请输入: " ans
来源：http://hz.guowangkeji.top/gtkncwfqiv.html

[R78] 交互式菜单
来源：http://hz.ydjk.org.cn/gtocuqfede.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jiagoushi.top/gtocltbjzj.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gtanaigrcd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gtwdeehnjt.html

[R80] 查看脚本执行耗时
来源：http://hz.zhaomingkeji.xyz/gtmeghubma.html

time ./run.sh
来源：http://hz.hysaishi.cn/gtczraqxez.html

================================================================================
来源：http://hz.kuanghao11.cn/gtlhxtxedf.html

S. C / C++ 专题
来源：http://hz.hfpthk.cn/gtipfdpcds.html

================================================================================
来源：http://hz.andypj.xyz/gtllxpbtmk.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gteokwrpmg.html

#include <stdio.h>
来源：http://hz.tianlin.xyz/gtcpcafvue.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jlsjyb.cn/gtcoemxlss.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtmsspjbcf.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtflvfkyxa.html

[S03] C：读入整数
来源：http://hz.yuanzhike.top/gtsunjjqqu.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gtohmdkzcp.html

[S04] C：字符串复制
来源：http://hz.jyoumei.cn/gtnxduksdg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xylfe.cn/gtqrbmvbue.html

[S05] C：字符串长度
来源：http://hz.jinghuilouyu.cn/gtznmfyqyq.html

strlen(s)
来源：http://hz.shuidangran.top/gtsgkxycou.html

[S06] C：字符串比较
来源：http://hz.shuidangran.top/gtqrmxthwt.html

strcmp(a, b) == 0
来源：http://hz.feifeiyinyue.top/gtbaqtgoyx.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtmpigbmop.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnxiangtu.top/gtzlqwquww.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigufen.top/gthpviwoxk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hfpthk.cn/gtzvjwifxj.html

[S09] C：结构体定义与初始化
来源：http://hz.jyoumei.cn/gtwrzykylu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hammf.cn/gtyscevdfl.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtmvbroacp.html

int *p = &a;  *p = 5;
来源：http://hz.feifeiyinyue.top/gtppvwmwup.html

[S11] C：逐行读文件
来源：http://hz.jlsjyb.cn/gtncuogcun.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhaomingkeji.xyz/gtkwwnlfqe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhijiandao.cn/gttkkxiodk.html

fclose(f);
来源：http://hz.gogol.net.cn/gtccwidsgq.html

[S12] C：写文件
来源：http://hz.c1oappe.top/gtozadzlvx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hysaishi.cn/gtoxdsbauk.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gttopwbili.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ywan-chungtsiang.top/gtbruyqsyu.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtnrkjmnoh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtyouembts.html

[S15] C：类型转换
来源：http://hz.jinqigfzy.top/gtdupxhsbs.html

(double) a / b
来源：http://hz.birdmap.top/gtxpfoaxct.html

[S16] C：位操作置位
来源：http://hz.haohaochexian.top/gtkguhqizk.html

x |= (1 << 3);
来源：http://hz.cashguo.top/gtnrsqussl.html

[S17] C：安全拼接字符串
来源：http://hz.zhoulong.xyz/gtbxkmprvx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yuanzhike.top/gtybqdnfxb.html

[S18] C：命令行参数
来源：http://hz.yj202588.top/gtndadmjdd.html

int main(int argc, char **argv)
来源：http://hz.gaohongyu789.top/gtqdkvhief.html

[S19] C：快速排序
来源：http://hz.chenzaomai.com/gterdypind.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtdtjimfiy.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtxxrvtmxt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhiwuduotai.top/gtekugedfk.html

[S21] C：字符类别判断
来源：http://hz.andypj.xyz/gtpnjzvshn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenjidiqi.icu/gtbmkkpqvz.html

[S22] C：字符串转数字
来源：http://hz.jinqigfzy.top/gtwkvrlcex.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258.top/gtkbunfiee.html

[S23] C：随机数
来源：http://hz.dianchejie.cn/gtuqxvgnnn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.9152youxi.cn/gtqufwluia.html

[S24] C：获取本地时间
来源：http://hz.hfpthk.cn/gtardezcjv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhoulong.xyz/gtwitvtcko.html

[S25] C：内存拷贝
来源：http://hz.dashuyun.cn/gtbamrdkxk.html

memcpy(dst, src, n);
来源：http://hz.jqgfzy.top/gtgqzqwmky.html

[S26] C：内存清零
来源：http://hz.birdmap.top/gtbbhunkpf.html

memset(a, 0, sizeof a);
来源：http://hz.zhaomingkeji.xyz/gtmwwtspfs.html

[S27] C：定义常量
来源：http://hz.aizwys.cn/gtxhcmvukf.html

const double PI = 3.14159;
来源：http://hz.guannengcc.top/gtoouojbcx.html

[S28] C：静态变量
来源：http://hz.dianchejie.cn/gtidflktdd.html

static int counter = 0;
来源：http://hz.jianghu66.top/gtshhoerdi.html

[S29] C：变参函数
来源：http://hz.fengsongda.top/gtyzcecchq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtsjtdzcjz.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangkeji.top/gtpbouenwn.html

#ifndef X_H
来源：http://hz.jinyuanbaomall.cn/gtgwwjuaqe.html

#define X_H
来源：http://hz.jinyuanbaomall.cn/gtrjkjylqm.html

#endif
来源：http://hz.c1oappe.top/gttlxhntny.html

[S31] C++：Hello World
来源：http://hz.yongpay.top/gtemhnrmjk.html

#include <iostream>
来源：http://hz.haohaochexian.top/gthvzbcwlh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhiwuduotai.top/gtdowufmbo.html

[S32] C++：字符串
来源：http://hz.yongpay.top/gtzblcutex.html

std::string s = "hi";  s += "!";
来源：http://hz.aizwys.cn/gtpngvphyk.html

[S33] C++：vector 增删
来源：http://hz.redwolf501.top/gtdqwopdxn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fengsongda.top/gtbmyooyen.html

[S34] C++：遍历 vector
来源：http://hz.dianchejie.cn/gtwxppfgmp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtgvpkfgcn.html

[S35] C++：map
来源：http://hz.shzxlz.cn/gtxrxodbet.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtamnczspd.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gttzidsokh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtteummhup.html

[S37] C++：set
来源：http://hz.yj202588.top/gtfikgdasi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aibaodan.cn/gtiadgjsdr.html

[S38] C++：排序
来源：http://hz.nanxuanxn.top/gtduywbned.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtiwdqprcg.html

[S39] C++：自定义比较器排序
来源：http://hz.zycfv.cn/gtndcnehcv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj202588.top/gtgvzsplys.html

[S40] C++：查找元素
来源：http://hz.tianlin.xyz/gtetdmrqvh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hysaishi.cn/gtcgdzprvb.html

[S41] C++：类与构造函数
来源：http://hz.chenlongwang.top/gtkcivompm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ivvv.top/gtpkagmnis.html

[S42] C++：继承与虚函数
来源：http://hz.52xcode.cn/gtrdnrkoga.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtbqtoxmly.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gtjyrklldn.html

auto p = std::make_unique<int>(5);
来源：http://hz.aizwys.cn/gtnctnhceo.html

[S44] C++：引用传参
来源：http://hz.9152youxi.cn/gtnyvwiudc.html

void inc(int &x) { ++x; }
来源：http://hz.birdmap.top/gteibrwfwy.html

[S45] C++：lambda
来源：http://hz.xuetiantiany.cn/gtcaopcipt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydjk.org.cn/gtfuasgxok.html

[S46] C++：函数模板
来源：http://hz.jinyuanbaomall.cn/gtigczbsko.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guannengcc.top/gtuwvqghau.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigfzy.top/gtmittagxj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxinkj.top/gtrkfctits.html

[S48] C++：逐行读文件
来源：http://hz.jianghu66.top/gtsrtygvar.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nanxuanxn.top/gtqxkhwqzg.html

while (std::getline(in, line)) { }
来源：http://hz.cheryme.top/gtpilntovo.html

[S49] C++：写文件
来源：http://hz.jyoumei.cn/gtbeqwckex.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shuidangran.top/gtnfztmmrv.html

[S50] C++：格式化数字
来源：http://hz.dianchejie.cn/gtscktjkyk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuanzx.com/gtedctajma.html

[S51] C++：显式类型转换
来源：http://hz.9152youxi.cn/gtkoqneuxv.html

static_cast<double>(a) / b
来源：http://hz.pycfn.com/gtqizivhxx.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgufenzy.top/gtuwosuyzr.html

int size() const noexcept { return n_; }
来源：http://hz.aizwys.cn/gtyyiqjxet.html

[S53] C++：移动语义
来源：http://hz.feifeiyinyue.top/gtbeihhdwt.html

std::vector<int> w = std::move(v);
来源：http://hz.cqqwz.cn/gtmtvlmtlw.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtiscxwljf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gtqjtymopb.html

[S55] C++：结构化绑定
来源：http://hz.yanxiufei.cn/gtehedazrr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenlongwang.top/gtndnoagac.html

[S56] C++：optional
来源：http://hz.snrcjt.cn/gtpbthoebm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.meibo888.top/gtqjqipohu.html

[S57] C++：编译期常量
来源：http://hz.zhijiandao.cn/gtdxiorbyl.html

constexpr int N = 10;
来源：http://hz.hysaishi.cn/gtfmrbhrep.html

[S58] C++：命名空间
来源：http://hz.gotoacloud.top/gtwjqtfxjl.html

namespace ns { int f() { return 1; } }
来源：http://hz.yvedp.cn/gteacyqhwl.html

[S59] C++：静态断言
来源：http://hz.yj20258.top/gtfsckskyp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gzhubu.top/gtfuxyjjvm.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtcfcfmaop.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtaolduvjn.html

================================================================================
来源：http://hz.shzxlz.cn/gtgqvivjvb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtqyyidlkc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtcrixyizo.html

[T01] Kotlin：Hello World
来源：http://hz.tianlin.xyz/gtlvivvxad.html

println("Hello")
来源：http://hz.snrcjt.cn/gtlwrztwdy.html

[T02] Kotlin：变量
来源：http://hz.chenzaomai.com/gtthoabpcy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinqigfzy.top/gtnssahzhq.html

[T03] Kotlin：字符串模板
来源：http://hz.meibo888.top/gtsotgmcet.html

"值: $b"
来源：http://hz.chenlongwang.top/gtpoaehvqc.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtbcdbnuss.html

val n: String? = null;  n?.length
来源：http://hz.zhiwuduotai.top/gtevmlnltg.html

[T05] Kotlin：when 表达式
来源：http://hz.wangshuangyany.cn/gtrpbqaftu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuxming.cn/gtffqzqsur.html

[T06] Kotlin：集合映射
来源：http://hz.xuanzx.com/gtbgufdqsk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.guannengcc.top/gtmezguxuk.html

[T07] Kotlin：集合过滤
来源：http://hz.daxiang520.top/gtgpapfgwj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hysaishi.cn/gtcqhfdwqp.html

[T08] Kotlin：数据类
来源：http://hz.zhengqikj.top/gtezdcdufy.html

data class User(val name: String, val age: Int)
来源：http://hz.zhongyouzk.top/gtrfrtdmob.html

[T09] Kotlin：扩展函数
来源：http://hz.xuetiantiany.cn/gtshnwswgt.html

fun String.exclaim() = this + "!"
来源：http://hz.fengsongda.top/gtksojjmgw.html

[T10] Kotlin：默认参数
来源：http://hz.cqqwz.cn/gtfhebabrj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yangfankeji.com/gtaopsakna.html

[T11] Kotlin：协程
来源：http://hz.ydjk.org.cn/gtgflbzkbn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydjk.org.cn/gtmjsvzcht.html

[T12] Kotlin：解构声明
来源：http://hz.xylfe.cn/gtphlhbqiz.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhiwuduotai.top/gtixtqpamq.html

[T13] Kotlin：只读 Map
来源：http://hz.wangshuangyany.cn/gtrqbyzhyt.html

val m = mapOf("a" to 1)
来源：http://hz.shanyushiyangtech.top/gtgvhuxwhp.html

[T14] Kotlin：循环
来源：http://hz.jinqigfzy.top/gtzqnardri.html

for (i in 1..10) println(i)
来源：http://hz.9152youxi.cn/gtrmctysrj.html

[T15] Kotlin：接口
来源：http://hz.zhijiandao.cn/gthigzghay.html

interface Shape { fun area(): Double }
来源：http://hz.cashguo.top/gtemvqgijm.html

[T16] Swift：Hello World
来源：http://hz.gaohongyu789.top/gtuolqaflj.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtfbkemwza.html

[T17] Swift：变量与常量
来源：http://hz.dashuyun.cn/gtfawprfhf.html

var a = 1;  let b = 2
来源：http://hz.chenlongwang.top/gtukbqcgqg.html

[T18] Swift：字符串插值
来源：http://hz.vqdsnc.cn/gtfvwjgryb.html

"值: \(b)"
来源：http://hz.yvedp.cn/gtlqwitdfj.html

[T19] Swift：可选绑定
来源：http://hz.zycfv.cn/gtokyrbjis.html

if let n = opt { print(n) }
来源：http://hz.zdqjudy.top/gthswwrnka.html

[T20] Swift：数组操作
来源：http://hz.sysykeji.top/gtpqmjnnlr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ivvv.top/gtkzacojoh.html

[T21] Swift：遍历
来源：http://hz.redwolf501.top/gttylnjhlj.html

for x in a { print(x) }
来源：http://hz.zhoulong.xyz/gttvdstryw.html

[T22] Swift：字典
来源：http://hz.zycfv.cn/gtxtootqzn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.haohaochexian.top/gtnzhxghlm.html

[T23] Swift：函数
来源：http://hz.yonumen.top/gtoefxwplo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xuanzx.com/gtahmueouu.html

[T24] Swift：闭包
来源：http://hz.cdnleiting.top/gtprvyqkwx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dianchejie.cn/gtfbvxhalo.html

[T25] Swift：结构体
来源：http://hz.gotoacloud.top/gtddkpkuum.html

struct P { var x: Int }
来源：http://hz.fengsongda.top/gttrfgqkun.html

[T26] Swift：类与重写
来源：http://hz.cheryme.top/gtcshxrddl.html

class A: Base { override func f() {} }
来源：http://hz.jianghu66.top/gtdarnupah.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtbzqryrce.html

do { try f() } catch { print(error) }
来源：http://hz.shangyingyoupin.top/gturvqxchn.html

[T28] Swift：枚举
来源：http://hz.yvedp.cn/gttjnvkvml.html

enum Color { case red, green }
来源：http://hz.shangyingyoupin.top/gtaeahndra.html

[T29] Swift：guard 提前返回
来源：http://hz.zdqjudy.top/gtzjnupnmm.html

guard let x = opt else { return }
来源：http://hz.yangfankeji.com/gtxgsqbkow.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtguziawop.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgfzy.top/gtblmydbhd.html

[T31] Lua：Hello World
来源：http://hz.svipenyu.cn/gtshtyjfrr.html

print("Hello")
来源：http://hz.yonumen.top/gtsrufyjgn.html

[T32] Lua：局部变量
来源：http://hz.birdmap.top/gtvwqqflul.html

local a = 1
来源：http://hz.wangshuangyany.cn/gtjgsoyfft.html

[T33] Lua：表（数组）
来源：http://hz.hfpthk.cn/gtgvxpcilc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.havefunace.top/gtpjnveovq.html

[T34] Lua：遍历表
来源：http://hz.havefunace.top/gtcazvvjgr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.vqdsnc.cn/gtrsslnmsj.html

[T35] Lua：字典表
来源：http://hz.chenzaomai.com/gtnzftwrfg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinghuilouyu.cn/gtzrzjptaz.html

[T36] Lua：函数
来源：http://hz.svipenyu.cn/gtncvhqhhu.html

function add(a, b) return a + b end
来源：http://hz.yanxiufei.cn/gtmyegydbj.html

[T37] Lua：字符串拼接
来源：http://hz.zhongyouzk.top/gtvpkjuupd.html

"a" .. "b"
来源：http://hz.meibo888.top/gtzolfrhfv.html

[T38] Lua：条件
来源：http://hz.jianghu66.top/gtvzldmitz.html

if x > 0 then print("正") end
来源：http://hz.9152youxi.cn/gtnsvhvxar.html

[T39] Lua：模式匹配
来源：http://hz.c1oappe.top/gtosbdnxjg.html

string.find(s, "%d+")
来源：http://hz.zhengqikj.top/gtuatacdzh.html

[T40] Lua：元表
来源：http://hz.9152youxi.cn/gtilbvhoxs.html

setmetatable({}, { __index = base })
来源：http://hz.shangyingyoupin.top/gtfvazouyl.html


<!-- 参考信息 -->