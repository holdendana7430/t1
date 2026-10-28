代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.smart0.xyz/gtabkolppr.html

[R32] 参数个数校验
来源：http://hz.chenzaomai.com/gtxcwvxqha.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fzhhl.top/gtyzrbeipl.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtnkatylbd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shangyingyoupin.top/gtiuwhakgs.html

[R34] 退出时清理
来源：http://hz.yj202588.top/gtangmzyfd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtuhrrsmac.html

[R35] 后台执行并等待
来源：http://hz.ybcxt.top/gtxeuwohpa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gogol.net.cn/gtmnzkfbtr.html

[R36] 并发执行多个任务
来源：http://hz.yangfankeji.com/gtkommbjfk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shzxlz.cn/gtoadnmppm.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtysjpuwuc.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gttnjopmng.html

[R38] 管道串联
来源：http://hz.xylfe.cn/gtbdimwijo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pengpengdd.cyou/gtfyflvogx.html

[R39] 重定向标准输出与错误
来源：http://hz.smart0.xyz/gttghlyvqg.html

cmd > out.log 2>&1
来源：http://hz.kuanghao11.cn/gthdjjuqlf.html

[R40] 追加写日志
来源：http://hz.dashuyun.cn/gtasrpybdp.html

echo "log" >> out.log
来源：http://hz.daria6918.cn/gtuicerobe.html

[R41] 丢弃输出
来源：http://hz.snrcjt.cn/gtpmumfddm.html

cmd >/dev/null 2>&1
来源：http://hz.hnxiangtu.top/gtiokzwvnn.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtagyerrji.html

wc -l < a.txt
来源：http://hz.aibaodan.cn/gtzrirdnje.html

[R43] 按名字查找文件
来源：http://hz.nanxinkj.top/gtwrqsxhbn.html

find . -name "*.log" -type f
来源：http://hz.shzxlz.cn/gtzliewxyb.html

[R44] 按修改时间查找
来源：http://hz.tian-w.cn/gtdezqyegg.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtprkrfnop.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gtxgmajndo.html

find . -name "*.tmp" -delete
来源：http://hz.shuidangran.top/gtfotdqimy.html

[R46] 递归替换文件内容
来源：http://hz.jqgufenzy.top/gtuzxsbdle.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hysaishi.cn/gtfopzqhic.html

[R47] sed 单行替换
来源：http://hz.mhx1999.top/gtctfzwhim.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shangyingyoupin.top/gtdxfyncem.html

[R48] awk 取指定列
来源：http://hz.mhx1999.top/gtrgwmfwhq.html

awk '{print $1, $3}' a.txt
来源：http://hz.yanxiufei.cn/gtogkwania.html

[R49] awk 带条件
来源：http://hz.daxiang520.top/gtlvfexhki.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.iojbl.cn/gtealhjbmk.html

[R50] awk 求和
来源：http://hz.cdnleiting.top/gtcfzrbhdl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.birdmap.top/gtrdwreaje.html

[R51] 排序去重取前几
来源：http://hz.yvedp.cn/gtugksfxqd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gtfjqwnzut.html

[R52] 统计行数
来源：http://hz.vqdsnc.cn/gtxjhkrkyc.html

wc -l a.txt
来源：http://hz.daxiang520.top/gtpgaomfjt.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtcxrifiyo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pengpengdd.cyou/gtzyspazbm.html

[R54] 比较两个文件
来源：http://hz.ehwqpu.com/gtgnjxqglw.html

diff a.txt b.txt
来源：http://hz.guowangkeji.top/gttvohbzoi.html

[R55] 压缩与解压
来源：http://hz.mhx1999.top/gtyixnadlk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangdashe.top/gtqblrnxah.html

[R56] 远程拷贝
来源：http://hz.pycfn.com/gtdadkvmaw.html

scp file user@host:/path/
来源：http://hz.nwbrower.top/gtpsdjkjwy.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtroyenfgd.html

ssh user@host 'uptime'
来源：http://hz.guowangkeji.top/gtmxjbuduq.html

[R58] 下载文件
来源：http://hz.svipenyu.cn/gtnibpjlzb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtptxjcyjo.html

[R59] 发 POST JSON
来源：http://hz.dianchejie.cn/gtnwnsxbxt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.andypj.xyz/gtkrsflqde.html

[R60] 只看 HTTP 状态码
来源：http://hz.hysaishi.cn/gtqrptqauh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pengpengdd.cyou/gtjggyitpg.html

[R61] 磁盘占用
来源：http://hz.cheryme.top/gthpzfetsk.html

df -h;  du -sh *
来源：http://hz.hysaishi.cn/gtaaocefvm.html

[R62] 找最占空间的文件
来源：http://hz.ivvv.top/gtyxqevlxq.html

du -ah . | sort -rh | head -10
来源：http://hz.hongshengwenyu.top/gtazbgawhb.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtvvqijlug.html

free -h;  ps aux | grep nginx
来源：http://hz.ydjk.org.cn/gtcqdvdsax.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtvjraofmm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.pycfn.com/gtpnsbecao.html

[R65] 查看端口占用
来源：http://hz.bjfxy.top/gtcfdodrtd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.c1oappe.top/gtmuvpglnm.html

[R66] 定时任务
来源：http://hz.yanxiufei.cn/gtbaobrizt.html

crontab -e;  crontab -l
来源：http://hz.zycfv.cn/gtbhklocsg.html

[R67] 生成随机十六进制串
来源：http://hz.redwolf501.top/gthofnsjex.html

openssl rand -hex 16
来源：http://hz.shanyushiyangkeji.top/gtwpwsghby.html

[R68] 计算文件校验值
来源：http://hz.gogol.net.cn/gtllrndfcq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jlsjyb.cn/gtvttjzsvk.html

[R69] 生成随机密码
来源：http://hz.fzhhl.top/gtvsvbfxzn.html

head -c 16 /dev/urandom | base64
来源：http://hz.ivvv.top/gtycfiklep.html

[R70] 时间戳与互转
来源：http://hz.0kj1m.cn/gtvqjhimil.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtfnvnboyh.html

[R71] 日期格式化
来源：http://hz.zhongyouzk.top/gtjmutoihi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtrjtfgnqe.html

[R72] 等待端口就绪
来源：http://hz.jinqigfzy.top/gtawvtggsr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtwtbzvdxa.html

[R73] 分割大日志
来源：http://hz.yuxming.cn/gtjpvimffi.html

split -l 1000 big.log part_
来源：http://hz.hnxiangtu.top/gtopnrzczi.html

[R74] 批量重命名
来源：http://hz.chenzaomai.com/gtdfchdkjk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hywenlv.cn/gtqmhyhsqk.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtihoyskxq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtvikakrvs.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangkeji.top/gtgyzubckc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.52xcode.cn/gtrxjgpbtd.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtknuuqplj.html

read -rp "请输入: " ans
来源：http://hz.haohaochexian.top/gtstolydyt.html

[R78] 交互式菜单
来源：http://hz.iojbl.cn/gtqsakxnxn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258.top/gtldtaunng.html

[R79] 解析命令行选项
来源：http://hz.zhoulong.xyz/gtbnrnhgrx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtljwdrdmw.html

[R80] 查看脚本执行耗时
来源：http://hz.xuetiantiany.cn/gtibiuyqsu.html

time ./run.sh
来源：http://hz.jyoumei.cn/gtfeykmiof.html

================================================================================
来源：http://hz.cashguo.top/gtmqmxsrwd.html

S. C / C++ 专题
来源：http://hz.jinqigfzy.top/gtphgnssmd.html

================================================================================
来源：http://hz.tian-w.cn/gtdzopnesf.html

[S01] C：Hello World
来源：http://hz.meibo888.top/gtctpkrtae.html

#include <stdio.h>
来源：http://hz.snrcjt.cn/gtwujubdnj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuxming.cn/gtjxvitgyi.html

[S02] C：变量与格式化输出
来源：http://hz.ehwqpu.com/gtpznaucpe.html

int a = 10; printf("%d\n", a);
来源：http://hz.haohaochexian.top/gtrlkeyeag.html

[S03] C：读入整数
来源：http://hz.andypj.xyz/gtutzqofla.html

int x; scanf("%d", &x);
来源：http://hz.yangfankeji.com/gtsfprkojc.html

[S04] C：字符串复制
来源：http://hz.gzhubu.top/gtrgaazqbn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangshuangyany.cn/gtsbtjdgbt.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtchlqctlt.html

strlen(s)
来源：http://hz.aibaodan.cn/gttsqtqosr.html

[S06] C：字符串比较
来源：http://hz.jyoumei.cn/gtdrzxinba.html

strcmp(a, b) == 0
来源：http://hz.shangyingyoupin.top/gtyrwaewfl.html

[S07] C：数组遍历求和
来源：http://hz.kuanghao11.cn/gtpnoxttks.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gttqpkhall.html

[S08] C：动态内存分配与释放
来源：http://hz.zdqjudy.top/gtlzeqddvm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hammf.cn/gtlfdkbfgf.html

[S09] C：结构体定义与初始化
来源：http://hz.yongpay.top/gtxjmvdoac.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gtudjydzjp.html

[S10] C：指针与解引用
来源：http://hz.redwolf501.top/gtocitrtua.html

int *p = &a;  *p = 5;
来源：http://hz.xinyue.icu/gtinaomebb.html

[S11] C：逐行读文件
来源：http://hz.fengsongda.top/gtezuawrmx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gtgwevkgud.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258.top/gtjhblcnww.html

fclose(f);
来源：http://hz.shanyushiyangtech.top/gtmolummmx.html

[S12] C：写文件
来源：http://hz.tanke756.top/gtpivbupht.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinghuilouyu.cn/gtedptemlj.html

[S13] C：宏定义
来源：http://hz.hammf.cn/gtrjslhldp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cucudq.cn/gtnpectxlq.html

[S14] C：枚举
来源：http://hz.cheryme.top/gtsqttrhnx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sysykeji.top/gtqmkecddp.html

[S15] C：类型转换
来源：http://hz.xziqi.cn/gtngxlghai.html

(double) a / b
来源：http://hz.chenlongwang.top/gtcbhsfgvu.html

[S16] C：位操作置位
来源：http://hz.vqdsnc.cn/gtkoavpujw.html

x |= (1 << 3);
来源：http://hz.smart0.xyz/gtmvrjqygk.html

[S17] C：安全拼接字符串
来源：http://hz.yvedp.cn/gtetmieulx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hfpthk.cn/gtebtgrdzo.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gtzfhlbotk.html

int main(int argc, char **argv)
来源：http://hz.shuidangran.top/gtzxlducpj.html

[S19] C：快速排序
来源：http://hz.birdmap.top/gtgoexjlza.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtnsdourou.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtdpdmfxet.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gtvwcomjws.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtufcknfjd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.fengsongda.top/gtclbmznmc.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtkhdhkayn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daxiang520.top/gtpypquxug.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtfltsftng.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.316326.xyz/gtvipndpcl.html

[S24] C：获取本地时间
来源：http://hz.ywan-chungtsiang.top/gtixkzxlao.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.andypj.xyz/gtvtrzdibj.html

[S25] C：内存拷贝
来源：http://hz.zycfv.cn/gtolxffnwq.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtnguwvfla.html

[S26] C：内存清零
来源：http://hz.quarkkingdee.top/gtrzzncmhv.html

memset(a, 0, sizeof a);
来源：http://hz.chenjidiqi.icu/gtfupewduq.html

[S27] C：定义常量
来源：http://hz.ydjk.org.cn/gtsuwlahei.html

const double PI = 3.14159;
来源：http://hz.cheryme.top/gtujeitskk.html

[S28] C：静态变量
来源：http://hz.daria6918.cn/gtrhrdfawp.html

static int counter = 0;
来源：http://hz.jinqigufen.top/gthuwqoxie.html

[S29] C：变参函数
来源：http://hz.shzxlz.cn/gtswyixmvo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tanke756.top/gtmikfvxgf.html

[S30] C：头文件保护
来源：http://hz.yangfankeji.com/gtagoequdb.html

#ifndef X_H
来源：http://hz.aizwys.cn/gttmncgylf.html

#define X_H
来源：http://hz.chenzaomai.com/gtamyhozxq.html

#endif
来源：http://hz.yonumen.top/gtbvxukzbq.html

[S31] C++：Hello World
来源：http://hz.shanyushiyangkeji.top/gthfahtibz.html

#include <iostream>
来源：http://hz.iojbl.cn/gtfhmtohnf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtmcfzloul.html

[S32] C++：字符串
来源：http://hz.ydjk.org.cn/gtdhwwfobr.html

std::string s = "hi";  s += "!";
来源：http://hz.meibo888.top/gtuwqmnrcc.html

[S33] C++：vector 增删
来源：http://hz.c1oappe.top/gtdvhajqzo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cheryme.top/gtlaqrmcde.html

[S34] C++：遍历 vector
来源：http://hz.tianlin.xyz/gtokcfxuos.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigfzy.top/gthrwqopre.html

[S35] C++：map
来源：http://hz.jiagoushi.top/gtczifgboc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtplwjbcuy.html

[S36] C++：unordered_map
来源：http://hz.bjfxy.top/gtqldegiyy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gttfousyau.html

[S37] C++：set
来源：http://hz.ybcxt.top/gtzahsdhbi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.meibo888.top/gtsixmqond.html

[S38] C++：排序
来源：http://hz.daria6918.cn/gtkuyshfjq.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgufenzy.top/gtcgfjubnc.html

[S39] C++：自定义比较器排序
来源：http://hz.xinyue.icu/gtpgdrjrck.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fengsongda.top/gtssfzjiwi.html

[S40] C++：查找元素
来源：http://hz.jqgfzy.top/gtnaynhian.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daria6918.cn/gtgimzgxxu.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtgqyomqjg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.wangdashe.top/gtrfqitcqb.html

[S42] C++：继承与虚函数
来源：http://hz.fengsongda.top/gtjmakmtxk.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtygkwrzvb.html

[S43] C++：智能指针
来源：http://hz.jiagoushi.top/gtukjuvwfl.html

auto p = std::make_unique<int>(5);
来源：http://hz.jlsjyb.cn/gtyxkpjrek.html

[S44] C++：引用传参
来源：http://hz.cheryme.top/gtgijakhov.html

void inc(int &x) { ++x; }
来源：http://hz.jlsjyb.cn/gtdxydjltt.html

[S45] C++：lambda
来源：http://hz.zhijiandao.cn/gtkpqsklpa.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.9152youxi.cn/gthmitlpkx.html

[S46] C++：函数模板
来源：http://hz.sufxvd.cn/gtykkekmyk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gttmzpskav.html

[S47] C++：结构化绑定遍历
来源：http://hz.havefunace.top/gtkjbrlsiq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhengqikj.top/gtgvwonbxv.html

[S48] C++：逐行读文件
来源：http://hz.daxiang520.top/gtlauiebik.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.316326.xyz/gtxfbbwiwr.html

while (std::getline(in, line)) { }
来源：http://hz.nanxinkj.top/gtcxpmpzxz.html

[S49] C++：写文件
来源：http://hz.zhiwuduotai.top/gthbggxeuu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenjidiqi.icu/gthbewiquj.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gtmpxpvask.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xziqi.cn/gtjslnclyg.html

[S51] C++：显式类型转换
来源：http://hz.ppjwa.cn/gtgzwsevou.html

static_cast<double>(a) / b
来源：http://hz.redwolf501.top/gtmqnfflba.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gtrczxyeam.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gtrensyock.html

[S53] C++：移动语义
来源：http://hz.gotoacloud.top/gtuocjjnhz.html

std::vector<int> w = std::move(v);
来源：http://hz.ywan-chungtsiang.top/gtooppcxef.html

[S54] C++：异常处理
来源：http://hz.sysykeji.top/gtfbhrcnzi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinyuanbaomall.cn/gtbqugaalw.html

[S55] C++：结构化绑定
来源：http://hz.jinyuanbaomall.cn/gttjnadcuw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtdgueyaju.html

[S56] C++：optional
来源：http://hz.nanxinkj.top/gtythqfzjy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sysykeji.top/gtcjkatpmi.html

[S57] C++：编译期常量
来源：http://hz.zhoulong.xyz/gthhmzunzg.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtbixqplmd.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gtlxpvrmtl.html

namespace ns { int f() { return 1; } }
来源：http://hz.yvedp.cn/gtdjabzvko.html

[S59] C++：静态断言
来源：http://hz.hywenlv.cn/gthvhldqtd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jlsjyb.cn/gtuuntkded.html

[S60] C++：遍历并删除元素
来源：http://hz.xingfuxueyuan.xyz/gtgmjvjpgd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gthqlbdlkv.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtaogmgrxw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtnnvxqbsn.html

================================================================================
来源：http://hz.sxryk.cn/gtbwiexmmn.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtnhlijqxn.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtbngraczr.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gtczwsoqvz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtkvaflney.html

[T03] Kotlin：字符串模板
来源：http://hz.jlsjyb.cn/gtzbjqfhxo.html

"值: $b"
来源：http://hz.shuidangran.top/gtlwwijglp.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gtqxmvxxrd.html

val n: String? = null;  n?.length
来源：http://hz.cashguo.top/gtqwledxha.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gtuejrfmlg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jlsjyb.cn/gtmceffkzf.html

[T06] Kotlin：集合映射
来源：http://hz.svipenyu.cn/gtrhdytkoe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sweek.top/gtkwakikfa.html

[T07] Kotlin：集合过滤
来源：http://hz.sufxvd.cn/gtwjdnocng.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jiagoushi.top/gthdjcqgpu.html

[T08] Kotlin：数据类
来源：http://hz.hnxiangtu.top/gtcfznsegm.html

data class User(val name: String, val age: Int)
来源：http://hz.yvedp.cn/gtcfhqwqoe.html

[T09] Kotlin：扩展函数
来源：http://hz.xinyue.icu/gtpncltklz.html

fun String.exclaim() = this + "!"
来源：http://hz.yanxiufei.cn/gtucihvxay.html

[T10] Kotlin：默认参数
来源：http://hz.cheryme.top/gtuzahfiey.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtvdjjnqbv.html

[T11] Kotlin：协程
来源：http://hz.hnqzz.top/gtmzjtzrnq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gtfhxrguwx.html

[T12] Kotlin：解构声明
来源：http://hz.316326.xyz/gtahikjndu.html

val (a, b) = Pair(1, 2)
来源：http://hz.nwbrower.top/gteofbidbv.html

[T13] Kotlin：只读 Map
来源：http://hz.mhx1999.top/gtsdptkxha.html

val m = mapOf("a" to 1)
来源：http://hz.zycfv.cn/gtcnbqlkkw.html

[T14] Kotlin：循环
来源：http://hz.gzhubu.top/gtqtfncokh.html

for (i in 1..10) println(i)
来源：http://hz.tanke756.top/gtfmlfsttm.html

[T15] Kotlin：接口
来源：http://hz.aibaodan.cn/gtlufzsfrb.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtzvlppnho.html

[T16] Swift：Hello World
来源：http://hz.yj20258.top/gtszsikczm.html

print("Hello")
来源：http://hz.feifeiyinyue.top/gtiweuezlv.html

[T17] Swift：变量与常量
来源：http://hz.fzhhl.top/gtkxenokpr.html

var a = 1;  let b = 2
来源：http://hz.zhongyouzk.top/gtrgbabnlg.html

[T18] Swift：字符串插值
来源：http://hz.zhiwuduotai.top/gtbgjmywnx.html

"值: \(b)"
来源：http://hz.cheryme.top/gtnegrnngo.html

[T19] Swift：可选绑定
来源：http://hz.cheryme.top/gtdkpotonv.html

if let n = opt { print(n) }
来源：http://hz.snrcjt.cn/gtfwuurtit.html

[T20] Swift：数组操作
来源：http://hz.nanxuanxn.top/gtppfyohgv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangtech.top/gtxjpfnkvw.html

[T21] Swift：遍历
来源：http://hz.316326.xyz/gtcfazsgtl.html

for x in a { print(x) }
来源：http://hz.bjfxy.top/gtrrlootqw.html

[T22] Swift：字典
来源：http://hz.jqgufenzy.top/gtditdbsod.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinyuanbaomall.cn/gtyzomurnd.html

[T23] Swift：函数
来源：http://hz.cucudq.cn/gtmrdrbipd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yongpay.top/gtdllkflvv.html

[T24] Swift：闭包
来源：http://hz.hongshengwenyu.top/gtconbcmrk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258.top/gttureicsj.html

[T25] Swift：结构体
来源：http://hz.jinqigufen.top/gtxkgeifwa.html

struct P { var x: Int }
来源：http://hz.redwolf501.top/gtfjpefmkj.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtyfvenzuz.html

class A: Base { override func f() {} }
来源：http://hz.sysykeji.top/gtwlgxinzd.html

[T27] Swift：错误处理
来源：http://hz.svipenyu.cn/gtkuysqtvw.html

do { try f() } catch { print(error) }
来源：http://hz.iojbl.cn/gtddzihdes.html

[T28] Swift：枚举
来源：http://hz.sxryk.cn/gtoiujpyrx.html

enum Color { case red, green }
来源：http://hz.cucudq.cn/gtvxmlhrke.html

[T29] Swift：guard 提前返回
来源：http://hz.zhiwuduotai.top/gtuaaoppsx.html

guard let x = opt else { return }
来源：http://hz.pycfn.com/gtqikhaisn.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gtsojsxgct.html

protocol Shape { func area() -> Double }
来源：http://hz.hysaishi.cn/gtdrmbkhdp.html

[T31] Lua：Hello World
来源：http://hz.mhx1999.top/gtiteyulcd.html

print("Hello")
来源：http://hz.fengsongda.top/gtktewvbod.html

[T32] Lua：局部变量
来源：http://hz.aizwys.cn/gtnnvkczsk.html

local a = 1
来源：http://hz.zdqjudy.top/gtpoumxkul.html

[T33] Lua：表（数组）
来源：http://hz.52xcode.cn/gtdprymalt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gzhubu.top/gtfwsuzfhx.html

[T34] Lua：遍历表
来源：http://hz.tianlin.xyz/gtobesweaw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hammf.cn/gtmmpgnaql.html


<!-- 参考信息 -->